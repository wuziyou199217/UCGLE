#This file is part of software for the implementation of UCGLE method, under the supervision of Serge G. Petiton
#<serge.petiton@univ-lille1.fr>.
 
#Copyright (C) 2011—. Pierre-Yves AQUILANTI and Xinzhe WU <xinzhe.wu@ed.univ-lille1.fr> in Maison de la Simulation. 
#All rights reserved.
 
#Permission to use, copy, modify and distribute this software for personal and educational use is hereby granted
#without fee, provided that the above copyright notice appears in all copies and that both that copyright notice 
#and this permission notice appear in supporting documentation, and that the names of all authors are not used in 
#advertising or publicity pertaining to distribution of the software without specific, written prior permission. 
#Xinzhe WU and the author make no representations about the suitability of this software for any purpose. It is 
#provided "as is" without express or implied warranty.
 
#You should have received a copy of the GNU Lesser General Public License along with UCGLE.  If not, see 
#<http://www.gnu.org/licenses/>.

#For more information, contact with Xinzhe WU <xinzhe.wu@ed.univ-lille1.fr>.

ALL: all

CFLAGS   = -I${PETSC_DIR}/${PETSC_ARCH}/include -I${PETSC_DIR}/include -DDEBUG
SOURCEC  =  gmres_cycle.c gmres_solve.c kspsolve.c gmres.c gmres_precond.c
SOURCEH  =  gmres_cycle.h gmres_solve.h kspsolve.h gmres.h gmres_precond.h
CLEANFILE    = gmres_cycle.o gmres_solve.o kspsolve.o gmres.o gmres_precond.o

%.o: %.c
	@${CC} ${CFLAGS} -c $< -o ./$@

all: ${CLEANFILE}

include ${PETSC_DIR}/lib/petsc/conf/variables
include ${PETSC_DIR}/lib/petsc/conf/rules
