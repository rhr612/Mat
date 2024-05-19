% Clear workspace and command window
clear;
clc;

% Prompt the user for their student ID
student_id = input('Enter your student ID: ', 's');

% Display the entered student ID
fprintf('Student ID: %s\n', student_id);

% Define symbolic variables
syms n z;

% Define the sequence x[n] (example sequence)
% You can replace 'n^2' with any other sequence
x_n = n^2;

% Compute the Z-transform of the sequence x[n]
X_z = ztrans(x_n, n, z);

% Display the result
fprintf('The Z-transform of the sequence x[n] = n^2 is:\n');
disp(X_z);
