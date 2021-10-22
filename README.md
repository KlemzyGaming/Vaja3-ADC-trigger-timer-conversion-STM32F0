# Vaja3-ADC-trigger-timer-conversion-STM32F0

Glede na potenciometer na vaši ploščici izberite-obkljukajte ustrezni kanal/pin. Na zaslonu se vam mora usterzno pobarvati izbrani pin v zeleno barvo. Kaj se izpiše poleg pina?
ADC1_IN1

Aktiviramo samo zeleno LED diodo na ustreznem izhodu
PD12

V Clock Configuration spremenimo APB1 Timer clock (MHz) na 16 MHz (pritisnemo ENTER). Kaj opazite?
Program se samodejno prilagodi na nove podatke.

V razdelku TIM1, pod Counter Settings, bi radi časovniku spremenili frekvenco na 1 kHz, zato moramo frekvenco ABP1 Timer Clock preskalirati v polju Prescaler (PSC – 16 bit value). Koliko znaša ta vrednost?
16000.

Branje vrednosti želimo prikazati z utripanjem zelene LED diode na STM32f0 ploščici. Uporabite metodo TogglePin iz HAL knjižnice in zapišite ukaz: (pomagajte si z vajo 0a).
HAL_GPIO_TogglePin(GPIOD, GPIO_Pin_12);
