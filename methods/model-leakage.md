# Detect leakage in a predictive model

For every feature, record the time its value first became available and the time the prediction must be made. Check derived columns and joined tables as well as raw fields. A date stored on a historical row can describe when the row was updated rather than when the information was available.

Build evaluation splits that reflect real use. Hold out later periods for a forward-looking prediction. Keep related records together when shared entities would otherwise cross splits. Fit transformations and feature selection using training data only.

In an invented example, a model predicts whether an application will finish within seven days. A field updated when an application closes leaks the outcome, even if the exported table shows it on every historical row. Rebuild the features as of the prediction timestamp, remove invalid inputs, and reevaluate on the same holdout.
