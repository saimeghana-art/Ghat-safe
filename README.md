
function getWarningState(traffic) {
    if (traffic === "clear") {
        return "CLEAR — DRIVE CAREFULLY";
    }

    if (traffic === "ahead") {
        return "VEHICLE AHEAD — SLOW";
    }

    if (traffic === "risk") {
        return "HEAD-ON RISK — HOLD LEFT";
    }
}
