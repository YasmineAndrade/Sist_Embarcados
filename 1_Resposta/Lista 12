1. Quantos pipes serão criados após as linhas de código a seguir? Por quê?
(a) 2.

(b) 1.

2. Apresente mais cinco sinais importantes do ambiente Unix, além do SIGSEGV, SIGUSR1, SIGUSR2, SIGALRM e SIGINT. Quais são suas características e utilidades?
SIGCLD: Morte de um filho. enviado ao pai pela terminação de um processo filho
SIGALARM: Emitido quando o relógio de um processo para.

3. Considere o código a seguir:

#include <signal.h>
#include <unistd.h>
#include <stdio.h>
#include <stdlib.h>

void tratamento_alarme(int sig)
{
	system("date");
	alarm(1);
}

int main()
{
	signal(SIGALRM, tratamento_alarme);
	alarm(1);
	printf("Aperte CTRL+C para acabar:\n");
	while(1);
	return 0;
}
Sabendo que a função alarm() tem como entrada a quantidade de segundos para terminar a contagem, quão precisos são os alarmes criados neste código? De onde vem a imprecisão? Este é um método confiável para desenvolver aplicações em tempo real?
