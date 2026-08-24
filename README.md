
    mkdir -p .repo/local_manifests

    cat > .repo/local_manifests/roomservice.xml << 'EOF'
    <?xml version="1.0" encoding="UTF-8"?>
    <manifest>
    <project name="galaxy-m55xq/android_device_samsung_m55xq" path="device/samsung/m55xq" remote="github" revision="lineage-23.2" />
    <project name="galaxy-m55xq/android_vendor_samsung_m55xq" path="vendor/samsung/m55xq" remote="github" revision="M556BXXS4BYH2" />
    <project name="LineageOS/android_hardware_samsung" path="hardware/samsung" remote="github" revision="lineage-23.2" />
    </manifest>
    EOF
