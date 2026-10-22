代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fdahejrw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtneblg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eeukkiru.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pyslofvt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2trszilpc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slzthzof.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vacchqhl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qdzkrmiz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lppnvsuz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hkazixwx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqvqnckf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hjtyjrcn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iktglyeq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ixeysicm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yonhllou.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uqrdadbc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rhthbjba.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mwoqnnim.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fkluexro.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hpqfniub.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mcbxkgmh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pfeampbu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vyirfhcz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2myxptczu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uzzojrzv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wwhmnhps.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fbbfkbix.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lqbzcpik.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zzawlwqx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ywcvuydi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kdrwqoth.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbgbxtxa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2yucmcuqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zsvjqmmz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zekgojnm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgtchbs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ucwdgwft.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfucadjo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ividdrfl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2omzbybnn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tsaskvok.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2yyymaiwx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmxenq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lzogoica.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xfyiuslj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2khxqkgtl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oamauwts.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bihmgcbl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2miwrulqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywfhhxwo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lognebde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gghkwvlh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rfkjfnpb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgnzlxyi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpfwxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rqartlqg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oepfuqug.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojkxgtqt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jsgxvqyw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qboageds.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yadocjcv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2bltwecex.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uilwlwum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixoiocmq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tfqvyjgm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xyknvevg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aopuocyf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tqynjpaf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yroaflyc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2obwfebnr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gvoevuao.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lzxxwfgp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amnrkltp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgkjowy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vjmxntvt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qeijcqmx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkjicwi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ktysrwzp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eqomoupo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rilutxil.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjcjbrag.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hauqaboc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfuwoyaf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lfnznbwb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aidfctqy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wxzxtrdr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2oedflsei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2njelwqsl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lpnqgyep.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tfettdxh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2anritujw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmzjeni.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xnkmgkvn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tpqigkxq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ihfbwdfx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pcquyqkr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yimmugsk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gdumxlio.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xtwmpdtf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ghhaeibz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttoffapl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vrblgzqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2prpnlgeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yputmhnq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcdlxhbx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2foedgczg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qeaguqkx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lshumpas.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kolaaimu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mzafyncl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zdjfbsto.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bngdbngw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ndbbiumv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jwrjrvco.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbcluhz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vomtgptc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cartmcad.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zqdehrsi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zfbttuko.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izxawhjr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hkqkqmqd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2edtbgiib.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ruurcjpk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zxmhlwed.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gbrhzrff.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqryasee.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2njhtujku.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cavmalqe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oqbkzptd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efslnhid.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmruuvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hrnowqxd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zissweyi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2urnqabiv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fjlxnzat.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjncgjvq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgjuwurp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2goriamar.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cjuopzcz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbtgibeb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sujnucsz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2chzcnnfb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ciwzpjyw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iwxuceny.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2neqdfnhj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rlihgffj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hzwniyzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vcbenqho.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qsqoyoem.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wuufumyc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tnqycjwj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rbmuuzmf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wgzrrtdk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vyjdpnzr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qzysivbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxsyedqz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qhufydhk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tzgixawv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2htniijzj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pcfigdhk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ivdwclrm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yzbwzzjy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zfhlsqqk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2btvvfqvh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mimubvhc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wakrutcj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wsluajff.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lavndefx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kkonzfyi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2daheqiij.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zizolhla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ologfxlu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeywgjhw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2higifshn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzupdjn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yaexhsrx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hzjaulfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ycvqterj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xnrgcxny.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ylpbaarb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dawggxdh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ndvtrquc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckukcfms.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2raimixxf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxpnvzjr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yhddndss.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2puwlkngz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hfqfzeev.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xkyoucxk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtnebthr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lqanzmcz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hjyyqmij.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bciyomem.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dllsmgtr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2shzqysmz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jaixxfbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnmdfdhd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtkaifxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlxzfztq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lxngbvqu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2eyhogpvb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaaupzyf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aijkhldq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thtyajad.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jtekdfcq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2txshoopq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gafuhapn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2icgqwvvf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wedlgsjh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cgsytvix.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkkydywu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mpwzmibo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2owedeqhq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tbsyabiw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdfcbmgu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yidqvlot.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qtcoilfr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zciiachv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2khmlqvqs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qtnudomy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiohhgxi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lxaflfmh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tgpsyvxt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wfkxnyvb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vinbjzrl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hlqsjmob.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vtpxliob.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xamlaewm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cshmlpcm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2espzyper.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2thmgxmpf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2edvazevv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkjxyuct.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcfixoh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vulpwuwr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gagynqif.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ucdjqtse.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2irudmnuj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mdgsvzux.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fgtxtzvl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bttjdvfe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tdpraalt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bgbxjbdw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gmytbyes.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2onegrjds.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hppsvcqk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2iruybvyv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rocpxyuv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtjunpxf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zibhyejh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rgxunwzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkobssh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pjtaqwof.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hkcxorij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yxothpma.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qezpeull.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hiqoscay.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zmyjbnqb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozyhpdxg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2exagbopa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mbtkeahf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ztriyrpf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dvjovhtz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2puxvkwjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwfgdam.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dghkhtzk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujilwhpq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bkmdfbjl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmzxnth.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhbvcqzo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2emfuqifu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycdttdks.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wbyissom.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bunqkyxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rkssitjk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2evqnsyel.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2epphlvzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2unkswukx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eihaclnx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tannppxj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iehwdxlc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2plzsnytz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2khjeznfv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uvlzxjyn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2txqunlbv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nmmxxtgw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2koiumabz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wkdzfmxz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2doshwldf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hfaenqkp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bvfbhqlk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2alwerloy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ajzlodut.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2levjtotc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2arpoxqmv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xkftlpjm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zzfvewbm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2eketwrvn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nmogghja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lmoyxehd.html


<!-- 参考信息 -->