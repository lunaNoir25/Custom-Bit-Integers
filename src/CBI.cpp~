#include <iostream>
#include <string>

struct uint2_t {
	unsigned int val: 2;
};

std::string conv10_2(int num) {
	std::string b2{};
	
	while(num > 0) {
		if (num % 2 == 0) b2.insert(b2.begin(), '0');
		else b2.insert(b2.begin(), '1');

		num >>= 1;
	}
	
	return b2;
}

int main(){
	uint2_t num;

	num.val = 0;
	
	while (true){
		std::cout << "\033[2J\033[1;1H";

		std::cout << "Press Enter without any other input to continue the cycle." << std::endl;
		std::cout << "Press Enter with any other input to exit." << std::endl << std::endl;
		std::cout << "Base 10 (Decimal): " << num.val << std::endl;
		std::cout << "Base 2 (Binary): " << conv10_2(num.val) << std::endl;
	
		if (std::cin.get() == '\n') num.val++;
		else break;
	}

	return 0;
}
