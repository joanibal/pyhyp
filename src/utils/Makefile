#      ******************************************************************
#      *                                                                *
#      * File:          Makefile                                        *
#      * Author:        Gaetan Kenway                                   *
#      * Starting date: 04-05-2013                                      *
#      * Last modified: 04-05-2013                                      *
#      *                                                                *
#      ******************************************************************
HYP_DIR = ../..
HYP_COMMON_FILE = $(HYP_DIR)/Hyp_Common.mk
HYP_RULES_FILE  = $(HYP_DIR)/rulesSources.mk
include ${HYP_COMMON_FILE}
include ${HYP_RULES_FILE}
vpath %.o $(HYP_OBJDIR)


FF90_OBJECTS =	EChk.o\
		initPETSc.o\
		releaseMemory.o\

all:
	$(PMAKE)  src

clean:
	@echo "        Making clean in utils... "
	rm -f $(MAKE_CLEAN_ARGUMENTS)

src:	$(FF90_OBJECTS)
