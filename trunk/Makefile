EXEC=sopwith
OBJFILE=${EXEC}.o

%.o: %.cpp
	g++ $< -Wall -c -o $@ -O3 -s -DUNIX

${EXEC}:${OBJFILE}
	g++ ${OBJFILE} -o ${EXEC} -Wall -O3 `allegro-config --libs`

clean:
	rm -f ${EXEC} ${OBJFILE}
