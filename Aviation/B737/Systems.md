# Automatic Flight

## Vertical Navigation

- Pitch modes available during VNAV: <font color="#00b050">VNAV SPD</font>, <font color="#00b050">VNAV PTH</font>, <font color="#00b050">VNAV ALT</font>.
- A/T modes available during VNAV: <font color="#00b050">FMC SPD</font>, <font color="#00b050">N1</font>, <font color="#00b050">RETARD</font>, ARM.

- Ground VNAV criteria (VNAV guidance only available after 400 ft AGL):
	- Valid FP has been entered
	- Performance data has been entered and EXEC
	- Both FD on
- Climb VNAV:
	- A/T holds FMC thrust limit.
	- AFDS holds FMC target speed.
	- Level off happens at VNAV altitude or MCP altitude, whichever is lower.
		- If constrained by VNAV → VNAV PTH
		- If constrained by MCP Altitude selector → VNAV ALT
