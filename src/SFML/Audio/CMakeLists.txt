
set(INCROOT ${PROJECT_SOURCE_DIR}/include/SFML/Audio)
set(SRCROOT ${PROJECT_SOURCE_DIR}/src/SFML/Audio)

# all source files
set(SRC
    ${INCROOT}/Export.h
    ${SRCROOT}/Listener.cpp
    ${INCROOT}/Listener.h
    ${SRCROOT}/Music.cpp
    ${SRCROOT}/MusicStruct.h
    ${INCROOT}/Music.h
    ${SRCROOT}/Sound.cpp
    ${SRCROOT}/SoundStruct.h
    ${INCROOT}/Sound.h
    ${SRCROOT}/SoundBuffer.cpp
    ${SRCROOT}/SoundBufferStruct.h
    ${INCROOT}/SoundBuffer.h
    ${SRCROOT}/SoundBufferRecorder.cpp
    ${SRCROOT}/SoundBufferRecorderStruct.h
    ${INCROOT}/SoundBufferRecorder.h
    ${SRCROOT}/SoundRecorder.cpp
    ${SRCROOT}/SoundRecorderStruct.h
    ${INCROOT}/SoundRecorder.h
    ${INCROOT}/SoundStatus.h
    ${SRCROOT}/SoundStream.cpp
    ${SRCROOT}/SoundStreamStruct.h
    ${INCROOT}/SoundStream.h
    ${INCROOT}/Types.h
)

# define the csfml-audio target
csfml_add_library(csfml-audio
                  SOURCES ${SRC}
                  DEPENDS SFML::Audio)
