代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmippwzb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kcemfymf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fttctvkk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xmhwddiv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gmwweuwh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sfpcmuts.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgnlfaf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kmtdkaft.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pwlojvyn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ytxangcc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3edzqoatr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jlltbmhi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rqefyfdj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hnauhwnf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rcgxdjqs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3meglbzwg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nkconpvd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qecxibfm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kfdklzfx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gbftbybh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpodepg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oubnijyz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zllieeiu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3swnvabqh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jrfivxvo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mqkebjkx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zpcbdtxj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mccohade.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zwemmbum.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnybuazl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lgqremll.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pmzhfnfe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zdynipdc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgoyvzcm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lreeqpib.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3etjaxsgr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jeflvqmb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3snfnqyzq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lflklajm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wxruzrul.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cfkxsyfu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3odynubxs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ktzjhslz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pnlqlify.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3htblrpuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgmjsfjw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mcbjcfgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iluelavz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lrqotnpg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3diojtikn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wegkwmlw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xvtujkmu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gzuprggs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kachdhzn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bhomnxlr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tganwdjz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ldhigswc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mulzmuxa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gkoeqigc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3epusqjbr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bsqwonec.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lvtiopar.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gmnmvzgq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkbyeqi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hhopmlag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3buqbdwfv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vvkgidsf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xdhgwlgl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zpxhlopz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdsfpmpo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dfkfnrsu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjcjuacu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgivbebw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3meysbfoc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nbmoohnw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zsehtnwb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jmunnapy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wvoqgvie.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fioykpdo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eilxjtnt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nrqdhsez.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltipuvmw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cncuwrap.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3unxrcqul.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pnsgtpwo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uawudgrc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xyhitbls.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3onrfaopq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mjdmbueo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yicvlyqd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3smwkzemw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lqkadhnd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kooslgqf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vqpxwpvr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vrrtqeto.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ybjuwgkt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qfiyxabp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3treamkiy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jknphlqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3csxerbmf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yvmtrwmd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgvpswo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gprkcolr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pccmjjpz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbvhprbu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gekwbkmo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kkvszjzw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3thwcpwie.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hicgckhr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3chwalbui.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ydilabid.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lltlaxat.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mczkitje.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ipywxhsw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ghuchtbd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3azbrvjdb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3npdoprxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xalbgqyt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3imndxhbn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lvthoobm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vhbtkecp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3aarnzacs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jalgjfmp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvnvvhw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pnwxpdvq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhknscqh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhdpvyl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3emnrryie.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xolllipp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wvbvehiz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfkicbf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gkjiypvx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ohjdhwyg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zoggsmis.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3viuurjmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bqszitvi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zedvkizv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rzjsgudb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cgpyjiov.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tktjllhh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3chqvwula.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nruxztlq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lriotfng.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lywftsye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dyqiwnmh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3fylihyxc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iogjtbpz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fjkdtsqg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3iyyujfqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3flgxmpdl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlwmip.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lxrvlaqc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ekjmucsn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pcelkhoj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ucgyqjnp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ptdxyjzf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iobctxcr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jideglyt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eofoksda.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knvkrbji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gurnamwx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nnfsytaj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3eaznzsoi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3onpflfrg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mgqwcqbj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjzpxt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pdvrdzef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fegoeusc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vizmuxjy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oplbagvc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkoffmbs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3blwwqgrm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bswbbaov.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryyqvpdf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mtucyobv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uimcctov.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wfkhpkyf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ygcrldgl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3isvqqaht.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jaqacakf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjsgkndd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3moxqnzze.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oeisekol.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xqlgerwy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wkoctzeh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cpmvjake.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lreiagjh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xoqdiqga.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvalagow.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxylzog.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zlzauqtt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xuczrsoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaiguosw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ogejfdgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcnwqyla.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ighshdnt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gwduqzte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jtnoyizy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxvbwwsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uevlryij.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mmigqllc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zmctimlv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iiujxgnd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmrywkag.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ulubkyid.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hqwmdmxm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gllhcgas.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucactuoh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukhlsurx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ekamvsvk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3asgodxdk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3chbhdkoq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3apgsrwuu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3enogkytl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3evlfiwcq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3igcutxxi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wglftvzd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eibhhhyv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tprliahl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hvaymabu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vwoxygpn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3moqggehz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uealezkq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iikthusj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3erwusgae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqilyhui.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wkagfbiv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ebhcwwsy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bfeurmvg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxpmrfnw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tblmpsyu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ablpoqqh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lkswkxhj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mearwlpp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ocamltfx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xvxzeaxw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3amrfdbsa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cjfkxzlc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ngdkjapx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mpubncsa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sdlcawve.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wabqlxbv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3htueaxoo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rtmpmdij.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zglvdrnv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3guvlofmk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nmeahkex.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hahwtdny.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3huzwgtlq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jnmyedmo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bttetlqt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjltipix.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fiabufbc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qblwkfws.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rnxgmrva.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3irwjltsr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tghbmpuv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ljtjhuax.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gglpbfwt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hhftbmib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3daxhqrxz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lyvorxfc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pjhksppv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3egnduugd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eqsujxtj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjihudcb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhavhyt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rwsttlun.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpnpnrt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xtdzrsja.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fwybhakj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ozkufvti.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ievlflyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kekimmxq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yufgkhuy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3alraxkwh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cbofgvup.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3aescimmn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wzwilzmv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uclxyjhi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qleqggud.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pnlcocrq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hvjgkhkf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nuwzrvfq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pstlgtzs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ufkqeczu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uemzfrdy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ckuikxzj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gidrhcfh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3sfwvegyb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kscpwwfv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fslaniig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wwsehyrj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uyotowyg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vzicugme.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tshhgyix.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mqzxkhnk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qvoikcsi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yqcccqfc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3opwaghcw.html


<!-- 参考信息 -->