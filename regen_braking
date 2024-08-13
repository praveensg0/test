initial_velocity = 20; 
final_velocity = 0; 
braking_distance = 10; 
vehicle_mass = 1000; 

initial_kinetic_energy = 0.5 * vehicle_mass * initial_velocity^2; 

final_kinetic_energy = 0.5 * vehicle_mass * final_velocity^2; 

energy_dissipated = initial_kinetic_energy - final_kinetic_energy; 

energy_recovered = energy_dissipated; 

braking_efficiency = (energy_recovered / energy_dissipated) * 100; 

disp('Regenerative Braking System Analysis:'); 
disp(['Initial Kinetic Energy: ' num2str(initial_kinetic_energy) ' Joules']); 
disp(['Final Kinetic Energy: ' num2str(final_kinetic_energy) ' Joules']); 
disp(['Energy Dissipated During Braking: ' num2str(energy_dissipated) ' Joules']); 
disp(['Braking Efficiency: ' num2str(braking_efficiency) '%']); 

gravitational_acceleration = 9.81; 
work_done_friction = vehicle_mass * gravitational_acceleration * braking_distance; 

conventional_braking_efficiency = (work_done_friction / energy_dissipated) * 100; 

disp('Comparison with Conventional Braking:'); 
disp(['Work Done by Friction During Braking: ' num2str(work_done_friction) ' Joules']); 
disp(['Conventional Braking Efficiency: ' num2str(conventional_braking_efficiency) '%']); 

figure; 
bar([energy_dissipated, energy_recovered], 'b'); 
xticklabels({'Energy Dissipated', 'Energy Recovered'}); 
ylabel('Energy (Joules)'); 
title('Comparison of Energy Dissipated and Energy Recovered'); 

figure; 
bar([braking_efficiency, conventional_braking_efficiency], 'r'); 
xticklabels({'Regenerative Braking', 'Conventional Braking'}); 
ylabel('Efficiency (%)'); 
title('Comparison of Braking Efficiency');
