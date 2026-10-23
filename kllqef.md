代发 wailian999

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ahewbqaw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qukuyrab.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzyxfbuy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tkpxwfzp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xiwhdsbv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvlaaory.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xjonvsrz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqfhykrz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3swvcpqxr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3djqaseaf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qexvbhup.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yiclqcry.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ooqnudfj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qkdfkwsr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pjvngwfx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sagaolhx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgwnddl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jwpzrtjf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jyftnqdy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cwlmilou.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ttuxaiui.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zyuiecrl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hcepqkvq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ehneqbpl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wwbalagy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ddjvgwra.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yugbqiie.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ysiyiedm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3czbkghjz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvkrdpc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3trceqlfm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pcbtenxq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3izqyucab.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jslkrzeo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xpuwpyfh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3atpcbuvj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3codsisln.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fimfxjch.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vkjohbvq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gytloivr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wzyjqkin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpkfroie.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lyxkjnmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmueojdn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cdsgtzrb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fbyrcicu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfcxezbs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hxadkqci.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3begkrclu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qdlvoyek.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zgijrtsp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yhncmhsp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3opqtrzzz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3powsnbpu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dwownbsf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iilyxsqf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gjwcmwjb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ozeogpyu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pgnamsxk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vbzdaxzs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3drkoafnl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xmpznpdq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rjmxbdub.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3alubvicm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dhfgdkwv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrsakxcm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjycfjre.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nhsgnlfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lecokngj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dndjzdxw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pimvdngg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3atemzyux.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nciojzzh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xqzepvax.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnsomyl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqiygjt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fjdkbzob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hhovifhu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hdemdsqv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3coajifuf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oftdpkwf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dnukhxwf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsqvzcbm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hwewsina.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhvipua.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hzzfxpai.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mumwzvkp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3echloika.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xasseoxz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3upzjmxza.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lyefusvo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lcqdaqta.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dzoochvf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3odrhocmk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pnabswyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rqhrewvo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3clrddcrw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bkjmoguo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3yhetedji.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3beawdxbr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fixpvmat.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gsdtidvw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lpxnjjsj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egkooxza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3snprqmys.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ytqpsoaf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qqsgalts.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vzvdgqvz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xswblwog.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hssiiqfg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hsrchlvu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kwqkujtn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yedbuflb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sgngbmio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sqnskmur.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mmhkbstc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ailoexrd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdyvzfil.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgbaaunm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vbepklwp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xryzwjge.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jsorlofu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ajdclngp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zkokhkfu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpzsiebn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rydiffgy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uxyebjkj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3myefyprz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pwhiqxfu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xfnrgsub.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zonqusvo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wqbeooyi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3edhjjshp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fppvslvf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iozojyyk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qgocsoec.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qeapiubj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3chxbjnou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uvsqwqpz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kttkqjyt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jkwizguk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pgesetxf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nlyetxiw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdhkugvd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3razrrypr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jfbofmbf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ktqauvoc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wbjqfwzo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbghiumx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3arkbbzwa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3orcyjvko.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mvaahigy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3oseiequr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gzbyylaz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hdfimdwa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3izdlddqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqdwzcc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kzmdkule.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wixzpuqq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3abwtyjti.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3twriztra.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cysmgqyw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jfkslbtf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcvgbyt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlclrqyu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yszvsowa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3flrglmbb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chrswjmq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iouwemuw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfarlqpa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3nuatrosm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3haxmhror.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zvcfxsbc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uztsjvfr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tahhssmk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbqmrk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yjuilytr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3everzarp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rruzdhkh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3flvzfann.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3thznyeno.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vrnsvtne.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rcrnvrnq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3henxdmci.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxaacm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3renohjem.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3etbezemy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jhurtbvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gifissaq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mkixrbgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfamjwcm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hslvlcag.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pkfoafzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3heoxprxk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xpdmugkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oilabpaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrpqeekn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gujnyoam.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvxvtilz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3npqlzdtc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbwfvuga.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vqlasjas.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xbktwluk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kqbtkwdx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evstvuhf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ywsksris.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdufvrqb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bkovvqpt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lblrbfew.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nazqojhn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kbponqwj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kqxzxzgk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsuppye.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpvkhk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzxxgek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3upmukhsz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3latjoybz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yzmkxncd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iqbwjmqe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqchhgxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zubscuzn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3txusfjwl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3txbbjoet.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lryklzec.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fdjtuwhl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdeplkco.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3epsesgan.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sgpvryio.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jojxqbik.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uickxeur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ypeomjpx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kggkrpcc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tetbpfoq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dngtcukb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ihnccofs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qbklkzoq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bzynpplk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cfymoxxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehhluvru.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xlgbctpa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dipqghfe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xbdliqvn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tlngvbqo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3soysawfl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nyxdxzih.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xomrafzb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fnfpebbx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tehajgmi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xzaqnoem.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3awsoodgh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjvmfvew.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mxynoqjl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhggyst.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gcykesex.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uilonftm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ztuelijc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3byfznzlm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rfytludl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oybmersp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3smhvjepy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fdjciumf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mapqhdue.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3odcglnga.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tgstyyft.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldddjmmh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyaukze.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3npdzyqws.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ectyhbrx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3frmzdorg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xazrhunm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mbatasql.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lpcaksrn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xghgcmws.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qhfjtspm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qtkgrqpy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zzzwlged.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qialpuao.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zhbxipbe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kpirldtl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xlrmchzc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jlqbebzz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xakqycku.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bxiqkraq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jumpzwok.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qctwdxia.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sgjkwdeb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uattslda.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3otitbioa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ekcwhzzj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qohwpusy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rfybyhvg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ytbecqkn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jzpoxjpy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wudrpqhe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lcczzvid.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vksxtyzw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ujwzmxsr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gguwvgrw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dzndhdgj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3icedwzau.html


<!-- 参考信息 -->