from pycaption import SRTWriter, SCCReader

with open('EXAMPLE_FILE.scc','r') as f:
	result = SRTWriter().write(SCCReader().read(f.read()))
	print(result)
