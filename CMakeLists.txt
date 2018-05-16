cmake_minimum_required(VERSION 2.8.3)
project(car_msgs)

find_package(catkin REQUIRED COMPONENTS message_generation std_msgs)

add_message_files(
  DIRECTORY msg
  FILES

  sbgAccelerometers.msg
  sbgAccelerometersRaw.msg
  sbgAttitudeAccuracy.msg
  sbgBaroAltitude.msg
  sbgBaroPressure.msg
  sbgDeltaAngles.msg
  sbgDeviceStatus.msg
  sbgEuler.msg
  sbgGPSAccuracy.msg
  sbgGPSInfo.msg
  sbgGPSNavigation.msg
  sbgGPSPosition.msg
  sbgGPSTrueHeading.msg
  sbgGyroscopes.msg
  sbgGyroscopesRaw.msg
  sbgGyroTemperatures.msg
  sbgGyroTemperaturesRaw.msg
  sbgHeave.msg
  sbgMagCalibData.msg
  sbgMagnetometers.msg
  sbgMagnetometersRaw.msg
  sbgMatrix.msg
  sbgNavAccuracy.msg
  sbgOdoVelocity.msg
  sbgPosition.msg
  sbgQuartenion.msg
  sbgTemperatures.msg
  sbgTemperaturesRaw.msg
  sbgTimeSinceReset.msg
  sbgUTCTime.msg
  sbgVelocity.msg

  AllData.msg
  Position6d.msg
  OdoCalibration.msg
  RearWheelsPulses.msg
  RearWheelsOdo.msg
)

generate_messages(DEPENDENCIES std_msgs)

catkin_package(CATKIN_DEPENDS message_runtime std_msgs)
