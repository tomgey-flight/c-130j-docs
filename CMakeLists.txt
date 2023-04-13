cmake_minimum_required(VERSION 2.6)
project(C-130J-docs NONE)

include(UseLATEX.cmake)

add_latex_document(C-130J-Flight-Manual.tex
  INPUTS 1_aircraft.tex
         2_HDD_and_AMU.tex
         5_normal_procedures.tex
         6_appendix.tex
         glossary.tex
         license.tex
  IMAGE_DIRS figures/hdd
             figures/hydraulic
  USE_GLOSSARY
  DEFAULT_PDF
)
