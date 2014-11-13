PHP汉字转拼音类(UTF-8)支持转成带有声调的汉语拼音和无声调的以及汉字首字母。
1、本类仅支持UTF-8编码，汉字集有20848个汉字，简体繁体都支持。基本上是汉字都支持， 随便举两个字：【龖】【龘】
这两字都支持 还有什么字 不支持呢。 ^_^

2、本类支持转成带有声调的汉语拼音和无声调的以及汉字首字母。
演示如下：

    $Pinyin = new ChinesePinyin();
    $words = '中华人民共和国';
    //转成带有声调的汉语拼音
    $result = $Pinyin->TransformWithTone($words);
    //转成带无声调的汉语拼音
    $result = $Pinyin->TransformWithoutTone($words,' ');
    //转成汉语拼音首字母
    $result = $Pinyin->TransformUcwords($words);