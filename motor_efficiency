voltage = [100 100 100 100]; 
current = [10 10 10 10]; 
torque = [50 100 150 200]; 
speed = [500 1000 1500 2000]; 

input_power = voltage .* current; 

output_power = torque .* (speed * (2*pi/60)); 

efficiency = (output_power ./ input_power) * 100; 

figure; 
plot(torque, efficiency, 'bo-'); 
xlabel('Torque (Nm)'); 
ylabel('Efficiency (%)'); 
title('Motor Efficiency vs. Load'); 
grid on; 

disp('Motor Efficiency (%) vs. Load (Nm)'); 
disp([torque' efficiency']); 

figure; 
plot(torque, input_power, 'ro-'); 
xlabel('Torque (Nm)'); 
ylabel('Input Power (W)'); 
title('Input Power vs. Load'); 
grid on; 

figure; 
plot(torque, output_power, 'go-'); 
xlabel('Torque (Nm)'); 
ylabel('Output Power (W)'); 
title('Output Power vs. Load'); 
grid on; 
