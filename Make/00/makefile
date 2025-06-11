target:f1 f2 f3
	@echo ' $$@ = ' $@
	@echo " $$^ = " $^
	@echo " $$< = " $<
	@echo ' $$$$ = ' $$$$

f1:
	@touch f1
f2:
	@touch f2
f3:
	@touch f3
.PHONY:clean
clean:
	rm f1 f2 f3
