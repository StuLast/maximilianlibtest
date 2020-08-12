# Maximilan Lib Test Build on JUCE 6

## Dev Environment

Visual Studio 19 on Windows 10 Machine
Juce 6 Framework
Maximilian cloned 12/8/2020

##  Errors

Severity	Code	Description	Project	File	Line	Suppression State


Error	C2784	'const _Ty &std::min(const _Ty &,const _Ty &) noexcept(<expr>)': could not deduce template argument for 'const _Ty &' from 'unsigned __int64'	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071	


Error	C2782	'const _Ty &std::min(const _Ty &,const _Ty &) noexcept(<expr>)': template parameter '_Ty' is ambiguous	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071


Error	C2780	'const _Ty &std::min(const _Ty &,const _Ty &,_Pr) noexcept(<expr>)': expects 3 arguments - 2 provided	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071	


Error	C2664	'float maxiIFFT::process(std::vector<float,std::allocator<float>> &,std::vector<float,std::allocator<float>> &,maxiIFFT::fftModes)': cannot convert argument 1 from '_Ty *' to 'std::vector<float,std::allocator<float>> &'	MaximilianLibTest_App	C:\libraries\Maximilian\src\libs\maxiConvolve.cpp	109	


Error	C2672	'std::min': no matching overloaded function found	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071	


Error	C2780	'_Ty std::min(std::initializer_list<_Elem>)': expects 1 arguments - 2 provided	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071	


Error	C2784	'_Ty std::min(std::initializer_list<_Elem>,_Pr)': could not deduce template argument for 'std::initializer_list<_Elem>' from 'unsigned long'	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.cpp	1071	

##  JUCE 6 Project Setup

Full details of all lib paths included in project can be read from the .jucer file.

## Other Notes.
- This problem has occured whilst following Josh Hodge's YouTube tutorial https://youtu.be/wEDr-gJxc_I 


- The Maximilan synth class has been removed as per instructions.


- The structure of the Maximilian repo has changed since the video was released in Oct 2017.  However, all the components seem to still be available.


- maximilian.embind.cpp was also removed from the project as this was causing an error (Severity	Code	Description	Project	File	Line	Suppression State
Error	C1083	Cannot open include file: 'emscripten.h': No such file or directory	MaximilianLibTest_App	C:\libraries\Maximilian\src\maximilian.embind.cpp	7	
).  As this was not shown in Josh's 2017 tutorial, I "guessed" that it would no be required.


