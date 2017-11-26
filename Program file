
#!/usr/bin/python
import sys

with open(sys.argv[1]) as f0:
        # do some stuff.
        human_data=[h.strip().split('\t') for h in f0.readlines()]

print "Read", len(human_data), "alignments from", sys.argv[1]


human_asterick=[]
human=[]
for d in (human_data):
        if 'chr' in d[2]:
            human.append(d)
        else:
            human_asterick.append(d)        
print "human_asterick=",len(human_asterick),"human=",len(human)

f = open("human_asterick.sam", "w")

for d in human_asterick:
    f.write("\t".join(d) + "\n")

f.close()
