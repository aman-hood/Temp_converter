#include <stdio.h>

int main(){
    
    float temp_value;
    char temp_unit;
    
    printf("Temperature converter\n Enter value and Unit\n");
    scanf("%f %c", &temp_value, &temp_unit);

    if (temp_unit == 'K' | temp_unit == 'k'){
        float k_2_c = temp_value - 273.15;
        printf("%.2f Celcius", k_2_c);
    }
    
    else if (temp_unit == 'C' | temp_unit == 'c'){
        float c_2_k = temp_value + 273.15;
        printf("%.2f Kelvin", c_2_k);
    }
    
    else{
        printf("Invalid Unit");
    }
}
