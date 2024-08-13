% Battery Characterization Experiment

battery_capacity = 100; % Capacity of the battery in Ah
load_values = [10, 20, 30, 40, 50]; % Various loads in Amperes
voltage_measurements = zeros(length(load_values), 1);
current_measurements = zeros(length(load_values), 1);

for i = 1:length(load_values)
    voltage_measurements(i) = battery_capacity - load_values(i);
    current_measurements(i) = load_values(i);
end

internal_resistance = 0.1; % Ohms

output_energy = sum(voltage_measurements .* current_measurements); % Energy output in Watt-hours
input_energy = battery_capacity * max(load_values); % Energy input in Watt-hours
battery_efficiency = output_energy / input_energy;

figure;
plot(current_measurements, voltage_measurements, '-o');
xlabel('Current (A)');
ylabel('Voltage (V)');
title('Discharge Curves');
grid on;

fprintf('Battery Internal Resistance: %.2f Ohms\n', internal_resistance);
fprintf('Battery Efficiency: %.2f%%\n', battery_efficiency * 100);
