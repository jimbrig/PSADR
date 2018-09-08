# ADR Tools (WORK-IN-PROGRESS)

A Powershell based command-line tool for working with Lighweight Architecture Decision Records (ADRs).

"Lightweight Architecture Decision Records is a technique for capturing important architectural decisions along with their context and consequences. We recommend storing these details in source control, instead of a wiki or website, as then they can provide a record that remains in sync with the code itself. - Thoughtworks"

## Motivation

ADR-PS aims to help document architecturally significant functional and non-functional decisions through out solution lifetime to benefit current and future teams. I also hope to promote ADR-technique into greater audience with more choice of tools.

## Quick Start

ADR-PS is a powershell module you can import in a normal powershell session. The default destination directory is `doc\adr`.

1. Copy the adr.psm1 into your solution folder
2. Open Powershell CLI and import module

	```powershell
	/ powershell –ExecutionPolicy Bypass
	/ Import-Module .\adr.psm1
	```
3. Create an ADR repository in the current script location
	```powershell
	/ Adr-Init
	```
4. Create architecture decision record
	```powershell
	/ Adr-New "User powershell for creating ADR"
	```
5. Help
	```powershell
	/ Adr-Help
	```

## References

- http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions
- https://www.thoughtworks.com/radar/techniques/lightweight-architecture-decision-records
