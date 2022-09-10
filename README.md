# brainNetwork

example:
S: time series(size of (m,n))
p: model order

[ Y,A ] = X_Y( S,p );
X = zeros(m*p,m);
for channel = 1:m
    X(:,channel) = LAP_SBL_estimate(Y(:,channel),A);
end