# 1

::std::chrono::steady_clock::time_point startTime = std::chrono::steady_clock::now();
doWork();
::std::chrono::steady_clock::duration elapsedTime = ::std::chrono::steady_clock::now() - startTime;
std::cout << std::fixed << std::setprecision(9) << std::endl;
double duration = ::std::chrono::duration_cast< ::std::chrono::duration< double > >(elapsedTime).count();
std::cout << "Milliseconds: " << duration * 1000 << std::endl;
