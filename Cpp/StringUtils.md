## 字符串根据Seperator分割
``` c++
void explode( const string  &str, std::vector<string> &result, const char& ch) {
    result.reserve(8);
    std::string next;
    for (string::const_iterator it = str.begin(); it != str.end(); it++) {
        if (*it == ch) {
            if (!next.empty()) {
                result.push_back(next);
                next.clear();
            }
        } else {
            next += *it;
        }
    }
    if (!next.empty())
         result.push_back(next);
    return;
}
```

## 对比两个vector是否有交集
``` C++
template<typename T>
bool findCompare(std::vector<T>& vec1, std::vector<T>& vec2)
{
    if( vec1.size() == 0 || vec2.size() == 0 )
    {
        return false;
    }
    for ( int i = 0; i < vec1.size(); i++ )
    {
        for ( int j = 0; j < vec2.size(); j++ )
        {
            if( vec1[i] == vec2[j] )
            {
                return true;
            }
        }
    }
    return false;
}
```
