i changed this line in the sessionx.sh script.
from this:

	CONFIGURATION_MODE="$bind_configuration_mode:reload(find $CONFIGURATION_PATH -mindepth 1 -maxdepth 1 -type d)+change-preview(ls {})"

to this:

    CONFIGURATION_MODE="$bind_configuration_mode:reload(find $CONFIGURATION_PATH -mindepth 1 -maxdepth 1 -type d)"

Because I wanted to remove the preview from the configuration mode view
