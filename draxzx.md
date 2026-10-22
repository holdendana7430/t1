代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mdzioyxu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2iknvcsia.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uwpgdggt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2atagpvli.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2eglgzlft.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2stbnldxs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qkdzwjdm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rpgqhhos.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuswtm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2elhwmutw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bzelmfnq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2osbskpeu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lqhqpwwl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qppphhky.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzghracw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2upnfbtyg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2glcopeej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xqwxrgvj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mfyhkgva.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2snbusgeu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hhyvdyem.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fawciokv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nrlnbimn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2knqiieqs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2stnqudzi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vfewgzrk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhyjfffx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sujjzxyf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qaqeupwi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovkznwkd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pfglpapn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ryzwillh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2raapdqfq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ucndheau.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qgvllabc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kptgeqpm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wqwjrmzy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dheyvowk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dskbotgi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ucdmbspn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dthmpbex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2edjfadst.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gvvrmxkk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kbbmqmge.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjstlpu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zvqwkbes.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vpfoubyg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ysnfixkq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dmqzgyks.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyeckoq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gncdihxu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xeajffkl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ekwkpups.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eqtqhjrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2upnjdreo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eohfgkgn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cwtzfdsf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sxlzkbbt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zujfdrov.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jmxdsglh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dbipmzfi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oryemylk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ogylyciu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2azmhdzgz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2egtlthze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edemcidg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ahkeuorx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxckngbx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tfpqbjxp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cemfxmlb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdjrvdiq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oktjbpro.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojcbtkzs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2znwjhdry.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ttcfdqzm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkzoof.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbioqpea.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zzkgwwkw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qakpkkqt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfijixm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oryhtxmj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qvmzkbwy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rfbvbudq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2poxsfzpb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nwuiuief.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jzdrqwaq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2plcdapcf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2evpighoq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aqipbqfz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woxqxscf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhytvxaq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gknzivks.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wowvuhdm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pnondhsd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ietipijc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kuwyvwgq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2palibuiv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nrhzdqas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ndwexhcx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uzjlkkuh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uiumvqve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrwtnnc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2edmvhklb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcyywfpm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ioeoogef.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pqmotkhs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktkvylnh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ppsgwmjk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2expkgwsj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2flflnylb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjaqdsi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mhqxigej.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zpysutqf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hjewfxos.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yaukdown.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yswxgezi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2trwfruhw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vpriifau.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qoxzpluc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2grcjdycx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eaiyuryr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2uusnhxnd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvwmswcy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aoliabdk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mxqtzeth.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqssjis.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dqixvnso.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjpfeeeu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jvmerdku.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjpsudsh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwsaaz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dodiwudu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ssuuudpa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wadorgwl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxmken.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fiyyfdqa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2crrowfol.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2doqmpcrz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2klehfdwe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ohatnwjb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kvqzbqew.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhegiotj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hlqbufjg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgovahrk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2osjiirhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iimguzds.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ztqmdhtx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wblosxva.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2avycoauo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2odwzikej.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vkqbnyhe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2evtrplpk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yxouqleh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pzuzpoxn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cnvafuhs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ghpfrity.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tmizaghr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qudxthed.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lchatnbi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yoznntly.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mbgxnejb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wrzvgpbl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tmtmrqtu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pzeerjtd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yrvojpyg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fytahkzw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wetezpva.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mxnwqsfn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ombbcgry.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yufkpimp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mlfruqac.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xodtpbiq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xemmljmy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2stvjmavp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gnumpbqp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zdhrwmku.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qhavgtqw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cqmvqpvs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldiifzhf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uknxikji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tjsrbtux.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dnbribyu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zhuexiyn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qgbsjlta.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rfjvwsvb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nhohptfa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nsrvcinw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iyjkbnor.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irnsqypz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzigufw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppskqfno.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wivpdovy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brfatndd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cvanters.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2egajjzaa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ucsksppo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iuckgswl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2afolkxfd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iexefuoe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qflubdys.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qcwenvso.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cdfmvvev.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2spqkmudr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cdhssadf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qrcgwotc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ounjurmc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ejcndnsb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uuaiujjp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fsaetogh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wcqpakye.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cvcatcbl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bcfrfhyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aysyento.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2omiyuhxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcdhvthg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbmbxuay.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bvdmofcn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmijvrp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhoxfyyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lwvzrnoz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fkefgwnt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uodczwgd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgtealcl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xsekkoih.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zafvocfc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kvizejor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2toexpkwk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cklvbvwj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyizemlv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2etskdkwj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpwhlthh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2idgaxsqp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vzwkamfe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dayzzsfv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vadsmxjs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhwpnw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2unmzxaid.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnbbxxch.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hqjkeeoa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gsxjahje.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2slqwydzl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2biblhwvu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eillkttm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnxxnib.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xltcjbxu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wlfetwec.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dbchrqwj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tjgxaqql.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ptxtmile.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmuvgdq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dxfzpgfh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kzljhbsm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uchafpzb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fnnzfxqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xchmixzt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lsomvjdt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vjasfhcg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sgiwbpjk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bqzixcqw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jpqsdobt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2klxtwved.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ryihsncg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2halynjjg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qwwhthnb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tozinwzb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rxsdldhu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bfoekgck.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dwizfomj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fbomzize.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eoskyvpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxdfibe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cmxygqvd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfiveuc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2piltpcjr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtimozwb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mwjklacm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2djgbumwk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2feyicaqr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zajayktz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pofughnj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2thnxozeg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbynszje.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoqyilky.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fzvtezeo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fzhejhdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjcnrhqx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhfnbkq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2noxdhnhb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhsgzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2monshlkj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2otcdnkzy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gzwzmjcw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbznxnkm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvijmvsf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ralvavgy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nijlpoxk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2smpwxxie.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2poknlqmz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2khbdblzy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jlmfurty.html


<!-- 参考信息 -->