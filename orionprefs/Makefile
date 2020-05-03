include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = orionprefs

orionprefs_FILES = prefsRootListController.m
orionprefs_INSTALL_PATH = /Library/PreferenceBundles
orionprefs_FRAMEWORKS = UIKit
orionprefs_PRIVATE_FRAMEWORKS = Preferences
orionprefs_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/orionprefs.plist$(ECHO_END)
