# Smart-irrigation-system
# Smart Irrigation System
# Python Simulation Program

print("======================================")
print("       SMART IRRIGATION SYSTEM")
print("======================================")

# Moisture limit
MOISTURE_LIMIT = 40

# Input sensor values
soil_moisture = float(input("Enter soil moisture (%): "))
temperature = float(input("Enter temperature (°C): "))

print("\n----------- SYSTEM STATUS -----------")
print("Soil Moisture :", soil_moisture, "%")
print("Temperature   :", temperature, "°C")

# Irrigation control
if soil_moisture < 0 or soil_moisture > 100:
    print("\n❌ Invalid soil moisture value.")

elif soil_moisture < MOISTURE_LIMIT:
    print("\n🌱 Soil is DRY")
    print("💧 Water Pump: ON")
    print("🚿 Irrigation Started")

else:
    print("\n🌱 Soil moisture is sufficient")
    print("💧 Water Pump: OFF")
    print("✅ Irrigation Not Required")

print("\n======================================")
print("       MONITORING COMPLETED")
print("======================================")
