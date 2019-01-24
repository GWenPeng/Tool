erro:
    info = {'executable': str(pe.szExeFile.decode('utf-8'))}
    UnicodeDecodeError: 'utf-8' codec can't decode byte 0xb2 in position 2: invalid start byte

不是你的中文路径问题, 而是你的进程名有中文, 这行代码 processes = dict(_iter_process())遍历了你的进程列表