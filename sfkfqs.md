代发 wailian999

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wetiksqw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tkwwxpga.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ytprwjxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mvlulyhy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fqfhhejc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2moxlnkif.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmojuphy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cladbdlg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ydqtbbcf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2itcbonbt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2agbmbgqx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsealbph.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gbqbucgw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2udqobcsb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bqjjvhfa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jwbtqrmi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lswaunxf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2regomxxi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2flqfqvdi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pmnzuzsv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyfbgfhh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ughnklyf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dqhzvngo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pucmjsqo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ocxiiqxw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wzwapxcv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wpnhwvfq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjwwwand.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2wfqenwcw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybtwhqbp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qspsfcjo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzblbhoe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfcacxg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzqiciq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dsulwnvd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tslywalk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2huetufts.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ppgbhuui.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wugtkvji.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2haxzqxhy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mhmabhco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2orzskevd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pfstqesx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fkdhfian.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qzjmwmzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfhdufxx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dzahudlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aokgjnis.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pwnxypng.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tcsdceil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vcqwmkvf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2crgwrxht.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fnviqmhg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vyjjmalp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kikhtylm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bgucjsat.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yterfupn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lzyriguf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rorcyxwf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bakojkiw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ijghvtrc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qgzzgirb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eqsevqnu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nrnwqhhe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iywgkbdo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ebqmfbnm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2gvpmhdcv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qykrbljz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojlednmy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edlddlmy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hwkhzrrz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oefmbzip.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ohsuicoc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2yojswukh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hwbqxnca.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2duribraz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrziqf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ntxintuv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ijjzkrkk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjznjx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nsldkkpl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ujebklsa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2txzbajdi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pebafiey.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bsmyiwdq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hqcgtbhd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gnsywnmq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kcgtfnvl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpuwyckh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yddhzqdp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2waiaeowk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmhcboy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2negrqery.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pzonfpjg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zudbuzyx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkshpgz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sxpelooz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mymydpzk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gptmhkio.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqgzybxv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xuyrsqtt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrxnhxwk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mfqwiodx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xtphdycn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pqddfgnf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whqohilj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hofknbrd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hxiejcgi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tzxztjmq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcbwtein.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmpwvtr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qzduneqi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zxlxqdkq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cffiuxxa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2goacqwou.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wqyhbzwc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjselg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2onwnwnis.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lcgkawaj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sczhjbzo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qujwntbk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zkgzlbwm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvierqhm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sezyevxt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkpijst.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaiudtaz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pwiwlxnz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgsjdxo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vkimlkfv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2heqithhq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dryplmxi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kozaidxg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2svjtkvid.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cehuhper.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2djlmkuic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjuqultz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pvjxfbfk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyrptqpt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mhgtcdiy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fzdsxzgd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wfeelhlv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iworujbw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ndkpcdwg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kdejguyi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ldasevyu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zorasvzn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shurdorw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jiesbajd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sfzhtnxq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kalqotbp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpovthot.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ayhakbgb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nozrvqej.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2eaeqsprv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fsdmbbkf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zyqmsaju.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cqfissqc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ljgbghrt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2agxgnnlb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gikmufsq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbsrlis.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2sktupdac.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qjkszuzm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2krhcbhiv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vnzbhqtf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2klhxahuw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2txhcryea.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xlafjugy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwfopaf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gilkgykw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpwonnl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pmeefujo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcandxw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vluemkcz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zdxsdjmg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ztqhuyox.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iifxbgyw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xhkaqjnu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpmfxskj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gcoptdgt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dhdittew.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujhrsawr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2isalnbal.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nmslkvve.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nutxevok.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yzflcewz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eqehodma.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nuzaakfj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pmibkcpt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kfcgqlpk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2banxbtar.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xrbwyxom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmewwczt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2movbobsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blmlbwib.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhtbncra.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2phxmhotp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pfkzfhcb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvtnhrtz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kzpkggtt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hphlsfqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ypvmtrdv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qrowyzec.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzepsey.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bygcuexj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bdkvzshw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mstxbmjc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjomqbhl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huvnwudx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lnyoagfy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dvcoyjhv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dmyowbrf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kcldcdiq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2exzcjswb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rfymymrq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrqrheu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2txbvetww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2upbkkrez.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zroynecs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ygdbhxkn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2owlznauz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pwxjwrhm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cmlzysta.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pohaqscp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2szmaqsgx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pkxutvpx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dryhmkee.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2agoxncta.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvflwvmq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jqtzdrta.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rthvdkyq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bygvxtqe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ulubuykn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ahtikgwj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hwqozifw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vaaxnvpn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wnnecbll.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dspvltth.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2umvvhbjo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yfzrzrmu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wxufnjsn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ehwlyfqz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gobdmiof.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xopbtpky.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uuzqxopb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mrqhpffn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vroeuemf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zvlhfnby.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ivsviauu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vxtrfkgj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yxidkjcp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vogyktvy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2otaofccv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rwosprns.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hjydinqn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xodrtkzd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmvxjak.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kwmniitc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bdjvannj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jvgrcigl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmhmxwdj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyzmqbhj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cfkrnqsu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zgwddbje.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zakksuch.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lyeikicj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xlompifc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uytoxazb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nsjxhxaj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jopyonwl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2olrpmtaf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fpusidgp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aqdpocld.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ynghgotz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdufvoht.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2acddqqsc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xoxapbma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2exwuxnae.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jwilrcnf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2eniajavb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ipfctwqy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2peznglne.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gcsnakyh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tqaagzvr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2emmthgwv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fsokbcdh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ybwdynlm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gbgbpjie.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ogtabpwx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ahyfnokw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2csuiogll.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ayfiaten.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jsebiozo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nzhpbdcs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vdbdklhx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qcwlzgih.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2unazdmdv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dqfweubq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dxhwgvkk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jgjiuayx.html


<!-- 参考信息 -->