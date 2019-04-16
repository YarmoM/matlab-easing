# matlab-easing
Simple easing functions for MATLAB.

## Documentation
y = easing(t, b, c, d) interpolates at timepoints t between b and the
change in value c with a transition duration of d. By default, a linear
interpolation is used.

easing(..., f) uses interpolation function f, taking the following
values:
LINEAR
- 1 lin (default)
QUADRATIC
- 2 quadInOut
- 2.1 quadIn
- 2.2 quadOut
CUBIC
- 3 cubicInOut
- 3.1 cubicIn
- 3.2 cubicOut
QUARTIC
- 4 quartInOut
- 4.1 quartIn
- 4.2 quartOut
QUINTIC
- 5 quintInOut
- 5.1 quintIn
- 5.2 quintOut
SINUSOIDAL
- sinInOut
- sinIn
- sinOut
EXPONENTIAL
- expInOut
- expn
- expOut
CIRCULAR
- circInOut
- circIn
- circOut

When specifying the easing function, both strings and numbers are
accepted, according to the list above.

Examples
easing(5, 0, 10, 10); % Linear interpolation between 0 and 10
easing(0:100, 1, 1, 100, 5.2); % QuinticOut interpolation between 1 and 2
