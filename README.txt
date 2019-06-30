Based on Cellular Forms by Andy Lomas.

http://www.andylomas.com/extra/andylomas_paper_cellular_forms_aisb50.pdf


- This emscripten version doesn't support threads.
- openFrameworks "ofVbo::bind()" got slightly tweaked (enforcing vaoSupported = false; for emscripten) because dynamic binding in emscripten was too much of a hassle.
- "-s "BINARYEN_TRAP_MODE='clamp'"" is needed in the build flags.
- "-s DISABLE_DEPRECATED_FIND_EVENT_TARGET_BEHAVIOR=1" doesn't seem to do good.
