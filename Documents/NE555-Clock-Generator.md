# NE555 Clock Generator

Circuit diagram for a 555 timer in astable mode, which can be used as a clock generator. The frequency of the clock can be adjusted by changing the values of the resistors and capacitor connected to the timer.

![alt text](Timer-1Hz.png)


## Frequency calculation:
$$f = \frac{1.44}{(1k + 2 \times 6.8k) \times 100\mu F} = \frac{1.44}{14.6k \times 100\mu F} = \frac{1.44}{1.46} = 0.986 \text{ Hz}$$

### Error calculation: 

$$\frac{|1.0 - 0.986|}{1.0} \times 100\\% = 1.4\\%$$


#### **Result:** Acceptable for educational purposes. (within ±5%) 

## Duty Cycle calculation:
$$D = \frac{1k + 6.8k}{1k + 2 \times 6.8k}\times 100\\% = \frac{7.8k}{14.6k} \times 100\\% = 53.4\\%$$

#### **Result:** Okay. (within 40-60%)

## Period calculation:
$$T = \frac{1}{0.986} = 1.014 \text{ seconds}$$

High Time:
$$t_H = 0.693 \times (1k + 6.8k) \times 100\mu F = 0.693 \times 7.8k \times 100\mu F = 540.5 \text{ ms}$$

Low Time:
$$t_L = 0.693 \times 6.8k \times 100\mu F = 471.2 \text{ ms}$$

Check: 
$$t_H + t_L = 540.5 + 471.2 = 1011.7 \text{ms}  ≈ 1.01 s $$
#### **Result:** Acceptable. (within ±5%)