#include <stdio.h>

int main() {
	int sum;
	scanf("%d",&sum);
	
	int i;
	char name[sum][4];
	int ibreathe[sum],ipulse[sum];
	for(i=0;i<sum;i++) {
		scanf("%s %d %d",&name[i],&ibreathe[i],&ipulse[i]);
	}
	
	for(i=0;i<sum;i++) {
		if ((ibreathe[i] < 15) || (ibreathe[i] > 20) || (ipulse[i] < 50) || (ipulse[i] > 70 )) {
			printf("%s\n",name[i]);
		}
	}
	return 0;
}
