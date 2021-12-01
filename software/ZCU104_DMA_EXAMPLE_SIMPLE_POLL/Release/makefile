################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
ELFSIZE += \
ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf.size \


# All Target
all: ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf secondary-outputs

# Tool invocations
ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf: $(OBJS)  $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: ARM v8 Linux gcc linker'
	aarch64-linux-gnu-gcc  -o "ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '

ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf.size: ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf
	@echo 'Invoking: ARM v8 Linux Print Size'
	aarch64-linux-gnu-size ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf  |tee "ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf.size"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(S_UPPER_DEPS)$(C_DEPS)$(ELFSIZE) ZCU104_DMA_EXAMPLE_SIMPLE_POLL.elf
	-@echo ' '

secondary-outputs: $(ELFSIZE)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
