# Last Change: Wed Mar 05 09:00 PM 2008 J
from numpy.distutils.misc_util import get_numpy_include_dirs
from numpy import get_numarray_include
from numscons import GetNumpyEnvironment

env = GetNumpyEnvironment(ARGUMENTS)

env.AppendUnique(CPPPATH = [get_numpy_include_dirs(), get_numarray_include()])
env.AppendUnique(CPPDEFINES = {'NUMPY': '1'})

env.NumpyPythonExtension('_combine', source = 'src/_combinemodule.c') 
