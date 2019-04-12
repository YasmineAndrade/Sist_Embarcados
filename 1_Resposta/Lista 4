1. Script:
for i in {100..1}
do
echo "Numero do arquivo="$i > text$i.txt
done
echo "finish"

Chamada:
cd Exe_xhell
ls
chmod 755 01.sh
./01.sh

2. Script
n=0
for i in $@
do

if [ $n -eq 0 ];then
arg=$i
n=1

elif [ $n -eq 1 ];then
cal $arg $i
n=0
fi
done

Chamada:
chmod 755 cals.sh
./cals.sh MES1 ANO1 MES2 ANO2


3.  Script:
echo "Digite o mes do seu aniversario"
read m
echo "Digite o dia do seu anivesario"
read dia

echo -e "\n"

for i in {2019..2009}
do
echo "ano $i"
ncal $m $i | grep $dia

echo -e "\n"
done

Chamada:
chmod 755 Exc3.sh
./Exc3.sh
4
12

4. Script:

echo "https://github.com/DiogoCaetanoGarcia/Sistemas_Embarcados/raw/master/Aulas/01_Linux%20b%C3%A1sico.pdf
https://github.com/DiogoCaetanoGarcia/Sistemas_Embarcados/raw/master/Aulas/01_Linux%20b%C3%A1sico_Shell_Script.pdf
https://github.com/DiogoCaetanoGarcia/Sistemas_Embarcados/raw/master/Aulas/01_Sistemas%20Embarcados%20-%20Aula%201%20-%20Introdu%C3%A7%C3%A3o.pdf" > sites.txt

echo "Digite 1 para baixar os slides"
read baixar

if [ $baixar -eq 1 ];then
for i in {1..3}
do
var=$(cat "sites.txt" | grep -n ^ | grep ^$i | sed "s/$i://")
echo $var
wget $var
done
fi

Chamada:
chmod 755 Exc4.sh
./Exc4.sh
1

5. Script:
n=$1
echo "cd " > arq.txt
while [ $n != "0" ]
do
var=$(sed "s/$/../" arq.txt) > arq.txt
n=$(($n-1))
echo $n
echo $var
done
echo "saiu"
