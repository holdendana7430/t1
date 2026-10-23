代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bpftekde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmlkllxm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hslvbgcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glofrqqg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3mgfxjggv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3uawddila.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvophmp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pwkkiovc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ojqpqzcp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fdlxpnue.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3kuoalzux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jxtsseca.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3byndatrq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xpdkclho.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bwdqqbqd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvziriqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fbzvfryv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ckmwsmqh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3akdctofk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qojfvsvo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ycbfwoiz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wpfatxvs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xhlxorbe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pmzbfdfz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gorjeooi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3svmvapcm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bzkxmkjm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwubcdq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3riejydyc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3cqokzegk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ldkjfgjd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3opytmnhv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qahlqjdb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3phawldmk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3evprnsme.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oahsxddn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bfwcgtrt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nunrvnts.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vpzylkmk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvanlm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3blkhiack.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3arheskst.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3orteqshu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3njlsctqz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cimpmqrb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ibpwvqob.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sddwixox.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3flcjodrq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdsfyfe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jxxhtolm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nvrwwwgt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bqrcmgem.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gatozpiz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eryqiodl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbjnnj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wnqhcprj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvulhce.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3myimqics.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpsuzobt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jehoasor.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwsrmovb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdoosnfj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mllywqmx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xzuazdqm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zlbaztvv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpgpoqer.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwzfnrzz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vlwkymgm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ubpoaqoe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ghtnpuen.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ztmpaxdu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nnlpwygj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tgdsabwa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3avlbmjwp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bhytoamf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gaxizdrz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xllujuqf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bxuderzc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pjlnayiu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnrgapt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wgxwecyb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uxikkeuo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dcmuhfhi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pczvgvjx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kixfvdir.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uvnkrlyg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sjnfcadt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3inqycdlc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tublndwy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jjsjjtjq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bbcpmgso.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3djxnjbfn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vegwjaox.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcomrbt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3etvtbezu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eqvrurwy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tpzmsgeg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ktimtsye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uceiikob.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqivrhyc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3innaczxa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rvnvyxgi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkovzbll.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aeaxikqd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dkpgxyso.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ykjqsagp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ktuadrfh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xqyxfvvw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnoommun.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3aqhimhdg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gooisdxh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3otdrmiwf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bsyiphem.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oeuputml.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wvmbdnph.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gimdnqak.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cripqsev.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3uabhfsrf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hjyjdtym.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ixbrvnjo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rjdphlry.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xufcqrrt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vkdulfml.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbcvpum.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snwwnvha.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tfkxprdy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjshmmx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3drfxqrrl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aujsxhmi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcedrbcz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vvrqnopq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hslazyuu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3woquvcnz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dwnowcni.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3barbvqqk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ajihethr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tihhujim.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wkfpsthb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mdumksqs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xpcsbthd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ecorcsou.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jvbfvvsn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3erqceqfr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ofaseytj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rzvvbshm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ydvfkjag.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lxieqddq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3caybmjxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wovlaypn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tfxvtqvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idvpqius.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hxbisgag.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cnhdxyuq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oinnhzyf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cykotqmb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnvgirkd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3suruxevs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qhkixrmz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3isrngpqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xuqtosbw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bsgqyytp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3aygofsli.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tcjsklzf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbcobbdt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhixfxqc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wbtedkcq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gxmwcqlu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lhimgdko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3broqydao.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xohywroa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3czcjhkvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lxawozxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lzjbxzml.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rkmjmqrb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3euugunex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dwbauzwz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzqgswls.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lofpgbds.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pyisapfq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3siialvxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dfcsdqfj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wusmildg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ggchvxce.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lcoemnbj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rteujqvv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfvwlky.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfifwgu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3polvnxoa.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hnhduhrn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hixotcwj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jtimasmb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bkloyzjb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3aqrpqrsj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rdamporf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3evkntcha.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iivkfblz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jpbsoqhe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3keqibivs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3axlsphuc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3otyvuirs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhsjsynh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fkbdzumc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtuxyzb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ryxuntoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fnluqiwg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3avomngsc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kivjcfdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qefvslpc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjqakpv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ugobpamc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aqhfnaok.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ogphcxpf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xhrkxjxv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kxpblcim.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xlnhdwia.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3icrnbzar.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3iiuoabmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gomymsqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjguiog.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cqhapxmc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qnjhxmoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jpabpkbr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lbszdorv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xjdnoool.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rohbbuls.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bebvrkjq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3atouvozd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wbyabhds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tygefppc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3smrtwsne.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hkpajasw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wcileskn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gujqmpoi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dmfxlnnk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3szmvpenn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bfutmavj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yrdjebdj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxsrfwvh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pipjqqez.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bwznislp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tymcalgm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vgufxdtn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wvfruunw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hsktnddp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3apdyijkp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3evdtceep.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zdyzusbb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jaytyych.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cncwaacq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxtaokz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tyzyjmpm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lzbxncxt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jonhhmmc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jcoqzyrq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sjydbskc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yhzisaqy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpdtvi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dccprckl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3brudiyys.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xglqibdx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3krdojchq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3baochfbv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ntuotzuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vysnodxb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnckvpi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ppoxeerc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3boizukhy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gelvtiqh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3oefskrgx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bzrfztrc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wnicvvzj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3emrnynbh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmpywvnp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nhtitmjm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gnpyltmm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aihujuij.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mjskgumv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zumtqebd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jdawkrkt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3urdiynpu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3daiuewie.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvvikxmg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3meymbrlc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eawtpsle.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wtqxluzg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3urstjrej.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3azqmrkjv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ricqxdet.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qnddiajc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gdxosjvn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ghdtjfwi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdduzrao.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zxtxmefo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ekebqfag.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bpcwjiqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssyttwle.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ftykhorz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cieqnpey.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3utzkfuty.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3njsdmmmd.html


<!-- 参考信息 -->