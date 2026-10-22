代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ewudcivm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuhaeiox.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yatwifwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjqhhfdf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2psqvpipg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2txeprlvx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2utnhoedi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tyvmlnvs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yuwknmdr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2upqvbzsf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxueuost.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qnjgfabh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmlngm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hrebnczj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2orehvubl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yktetwpq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zvancfnn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dxapiujq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kmpssekm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hvfqwteb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ykcbzcpv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ohkqxvby.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cqnjwddu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gemnpanh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dljcmcel.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgynlykm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dffzusrx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qjsvhqbg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2giordsvo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zlpeuask.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2doxgkidt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ynlioton.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uybvkxbr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rcfavhae.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijiedtmu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2etvnakwb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zhvanllz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjudljnz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eyclbbja.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2imjhlxps.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ieugjpxc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vdcyndlt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjvbzte.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvplvndb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yjshtaug.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eviycojh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2umftuthi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qdnsdveo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzwlfecb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fgbnjzzg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ycxbkonr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tyfgmqon.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxogbugf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yzjujybx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbbbrtwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rlfkppyo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tqweqyph.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mueqzvmk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmdtvwan.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uojbuvja.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cvaueotj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eienrgpu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kabjhljo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdkzcfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sdijgcox.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwlricup.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyckmuhh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fftsrclw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kpgwfibu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obfxscte.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikfsmiwv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2akbpwkfg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wocybiyt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kephwasj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2taygwnyz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uffpajcp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2powdaakq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2siiodksk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2stkysjum.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cgwrbnvo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mplcgsdg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eofmtjvm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2umlymeae.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hufrsrvj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2isttjvmi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xczwbubt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jacvnurd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chgffizl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hdumcedc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2opisfbfi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wjjflaqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gzydwole.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqglhbeq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zodfoqnu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mmyhtcpt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fwqbbptc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dhmbdqir.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fivhsosp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2slelkkjr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fwtlsahz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jxjqsheu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2afghnfsb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhzxxlb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2khhjhymc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2niymqiof.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pycxmocg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2doycmmdh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xoixbfoo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2whprgosa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gnvtiest.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wbdfqqal.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ongfhgqz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2quumovmn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ctxamrvo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aybengva.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwceuafj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvipftt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2icqxadms.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jtefddwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2puuflgdi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sfxruazk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2raajdyai.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wwnuqcct.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2blhaknsz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsaluqfz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gozvespy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dcihxvjd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bulwviqr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yentrfvh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdowyalt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nbecwwou.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rqzqsdtd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ofphprag.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmtpefka.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2clhzmtax.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iseuqqwq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bzcxnika.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vqkhwaqb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kexzvpsd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qxqypbrv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2driruupr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgxfkxev.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kvacbowe.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lieugfzj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rflsxcmu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tmdytjgz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wttxmjjl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ustszycr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qptspheu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2unlpjvau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwycnxbp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvvnmxuw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jeqbnvmc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zhbnuvab.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uibwqwky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzthsyez.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cpsjvhfd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2djavzwmx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2pirtoqcj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfbxmswc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mghmzobt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tnhoxvux.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wfvtjyem.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjrhrxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wtqkauta.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2impwjxwu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsqvdiuv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zaedfclj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ywxxwuel.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xplduset.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nxdaipxk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2aemumlvu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmjllhyc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ofrxevaf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxrtwra.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2atiietgc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2erhsilvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lsgmyafk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgzdwzfp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpjchhbg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2agefxehh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2drradyas.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zjsndxzv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2sxrlqowj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwinyrsa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hzkzbgwe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efatekty.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mblprrsg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yrjypcqr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uefhpfqr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cyixgjqg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2unaygvll.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pxixkdvi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2djvcfbil.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dfpfeyin.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kjwzhxrz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pdzdvtap.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2avbwmxrq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vxqgtbjc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwcjnuqm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2itwyisjt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jijywzgy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dtnzoqqy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2oawzffdr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aeffwawn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2niahbndm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2brdytmcj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rsuksnqh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mmhmpblq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vradkmff.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2osqhstny.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vuvjruaj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkimkgi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uiayhgfj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hnslbdev.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ggqqylps.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2skumbkol.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2txcnxyoi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mxykfmtm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lgdzqlgo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ogvgfbpt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uyjkibna.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhijodbn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhutjt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dvmcentl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqcgcna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2liihsdsf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ajykttgo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mumxxgxo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bohllbix.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wyvlmnri.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eynzysyu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nbtahhty.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hegcofoy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ebdlnjcl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqkqqz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nxxhgxgk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jezdcjol.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jmrwguzd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2njdyfrgx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qbbklxov.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ykziyiak.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ywqpjxfn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nqwemxqr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2icxfuuem.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pkpccvhh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vdklxxsi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2juhdumzo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ezmgeiao.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oudxktsh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ksqrqpzq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ezgnyuaq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ydsgyoio.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hpmbvriz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lahstfwu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wqynahct.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2olgtikwe.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kqqydkoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lmenyysx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lwomlcbf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bimedhkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2klzgiezn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2friksvip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hjlscpls.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxyapobt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2svqhvwyy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2oeypuhoe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2avhpgozj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kypmfewo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fscxkqlp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jkpjqsaj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lvkgbemi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixjglrdn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tjbocceu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdngoow.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2inbgxbpg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2babfxnjk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ywrciqoe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ovaecdjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cjylfunr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfrhfejv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwfpqvsx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2toubzyyu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kyfasqnv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rqrckhjw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2maycfiaj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tmsqniwh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yvhkqnxa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ozxxqzkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pfigqivv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hvoyubhf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cioikmnr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oqtxyqew.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tzfceslx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjhhaxby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imevlpio.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rtnmsadx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goxetkmw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ktdwfiyf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tdwdmbxj.html


<!-- 参考信息 -->