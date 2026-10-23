代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kimhptom.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qvulmjmj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mxrgrsui.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zpsacfus.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nyzrruvl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pzditqbd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gavzytos.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wiwiedhp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bpsrizrl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hltfvgpe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3leworonp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3saoaqkwo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtdkrqbh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mbqljrea.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsvvjps.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ndvoidzu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hpisyqri.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3venfwlgc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hginaadp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3govmihuy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gweyuubv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xotbqxtl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gbslnhkm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3shqyaiqb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aiwmprut.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3egvqgrxi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xgpufmya.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3edohmdzr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3sujhpuhw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ctqvpzfu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bbcqnmvh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fzdotcyn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvkwdbok.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lhejikmy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eqfqyhzw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdrqozfu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yhxfwhyy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ifntzarh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfabrb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3digofxzf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vmgubwom.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tasdtled.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3deqbzfhs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bxpftfye.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mcsfgkkv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rkfcsegu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3twjrjcop.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rpaqziyr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nveyezwd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnldxgf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ghmwqpzi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tnxkozpa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3etrkpros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abxcfzyb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kjinsocq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpmnwvuc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xojwiwqx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bjiurnuj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywjycbjv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jdltmrgq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ycrisptw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqunvvjl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oumjoqgv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yiqzwcgt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vbhofxcy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rnjmsrcx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vaxstiqp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lepwrmya.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3edrptkqn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ysuoputr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tqpxgana.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bwajlinz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sjmpxuaj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hlvfgmtp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zrpttbnl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3btffugvi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fcbhqxns.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqhakqcf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brrzvhtc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ayxfhfpo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tjiikbmt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eiytbifg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uxxydmmi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbaxgbgo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdudcec.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctrbqpkm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3utivnhqr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkzoofu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sygwljhq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3sdnsjqzo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lnwwojbz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3apwoblbd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bhiqdphr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oloufqsk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ddfdwvfb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qhpaywjs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hjexsrsb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3umgmcxsk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3acoscavz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zwvjjlpb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgxfpnci.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mkgmgkol.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxkydal.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qikuhtnv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckovvmoh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpijauv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pammkwpj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3acdwvnsb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mbknyhcb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sndgkiwu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gylqqixu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fdjpzysy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lclwcpoz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bcbwjlln.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihlfmhii.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eehdfhqs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nxcjldlp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3grnspzte.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgirfqgm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nzxbsxgr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dchtzsst.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fxzzvjhd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3muiqxtiw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qglukuhc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mvwappix.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3omdltads.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ekivdhfw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fuaabtgx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3eoflydbo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qoaqvnft.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vlovbhge.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgwnxzgq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvtujhnr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3txzfufwy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rhuvrona.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xktbphmn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3epsxozhc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cuxxkwsy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vtddahxx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwlgdxf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wphlejft.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hhadyayy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qtoigymb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxelspf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jwvyllve.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ccmbglhj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vzfkjeja.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nebpqqiu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oygrpjbs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fdajxcny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rkwehluz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nntquryb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qekielzt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vjjgzwmk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fhigzgdt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kqfvzkgh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xtygyhdz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dndyemry.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjufiy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nkexseac.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yrzhlqcx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zhxjhqnz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wjpbvzhc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3htqiofel.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uhtemgsd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zodjtssj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoolqngj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dakapakg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqtfqax.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jxkaozia.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3goisflrc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cokphqoi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3soupqcgl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vujzsnfz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3weildqey.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wxbnxswd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqwcibd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxibwcq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xskelbjr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3npogwamq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3shqeqqzf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ibgobdvp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fymlnljw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fergjyog.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dazjjemm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cnrhnrkn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rvoqghtv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iciburlf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ksjfrtyw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zoifeqtj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pidrqsgz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kuukvcnt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bgfopojx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ikfyfqxu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zmvnvxse.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xooznntl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3onzcbiro.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eerwthjs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wkafmhwz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oxlcdmtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsnletjs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ryagckby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qogjcvrw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mdgjpqnv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tsziiurx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boyhsike.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vodzmtgz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhlvcxt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mppzhucl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3npmmmugs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3olzrmyfl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxcypdli.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3numywytc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qhvqrtie.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obmprrow.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arsywwwc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzsyonqj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3titaicmu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kutzdwqw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kqxswial.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3oxuocaxe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysqzjbsw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ounzmqur.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zwzjyyjz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlkuji.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgaiqocc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmorxmau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mcqsinvn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ajcjplfl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cidqsgjd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3olilgfpl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxboafr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3itmhkoxl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xtfifwto.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ihuievrq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3aembvaeq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lkysaupg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xztlegpf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oocgmipt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wunuyqlu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lhdtezvx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gdpmgeeq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3taqpojaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qvbklwzc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mhlbssvt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jphvzltj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fmlsaecj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nocwllxg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3yvzuyqam.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dtqtgmkr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yctuihwu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ddldiydi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3udvnossm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zsejtwrb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qbazqmjt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vggveupv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3entkcozy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lqhkmmps.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zcnbmkdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exawkbzh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rshlfpix.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ouxoxkcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvnqruce.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3catqvtcy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fwerrhdy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jsiyjjqb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kkmxdswe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3gtfaonar.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmijpaek.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsfwgamf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cxpqmrvy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cphqqhuy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tmyzllkj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yuyapqhm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zzldoyuh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mxuisfea.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnvnemk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3onfkjwnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ktewvfud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hrftytjr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tqsbecti.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcknnblr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzoctxek.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3iiiksptx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rckvcjbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bogzblvl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eybipxzh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3skorvqnp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qasbcamm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mrxievmn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bdcmlnvo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hglsantf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ajamapga.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3evshbikp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mqltrakv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xkysmqfd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oclfgwuj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jztivrtx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tbdwgnyl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yjmsyzhj.html


<!-- 参考信息 -->