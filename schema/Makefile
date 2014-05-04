## DOAD Schema makefile

.PHONY: live all

all:
	@echo "Type 'make live' to transfer the schema to the live site."

live:
	@cp doad.rdf doad
	lftp -e "open -u kamir http://semanpix.de/ns/; put doap;  quit"
	@rm doap
