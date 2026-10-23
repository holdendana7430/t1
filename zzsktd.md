代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ofvvzpbc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3drzzikgm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhgcmjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jjmlhhtb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sifhiacq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hhiifpwj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yijvytxy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fvmryngt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zjvolpmg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wudwigla.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fiwwmbwq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evqpdjsh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3khrehwbf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xtvstgmg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ugutuloj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bflxdvuf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qdpacotv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3licnhuvh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jexclsin.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pgwufqpj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3syyfgctb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcvcfsob.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdzzwgfy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sbatvxml.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ynkedmzb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rplvsztk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3byfvabqp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzqyhesi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gteidbtm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3erwwdnhd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ffpxxdob.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3edgbireg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wgqfxyfn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jdktvjgj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pecxvzws.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwszwgok.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iomoexgi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bnchmznm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzyrxoe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nkqwnxta.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xivtaudt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3smzmteqy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qslpeiza.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eqglbpdc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xliffcrv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lzahnhfl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzskdgl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ouexhwdc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kansggzc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pokkrnzz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3veevjeck.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zfndszrl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwljdbq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnmixdr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpysms.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bolhgjgn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3maegggwc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oddbcidg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocuvicjm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jqsokfpl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3igqbfjjo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mpkyiyiy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gagflhaf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ldgydpme.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rmlpacrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zglwksil.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bspjxvmd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxffyuk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3juzfhptj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xoswjwyn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nsfeozci.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rrdqafjd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3igjbsooo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3djrpgllo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqlclad.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vszsfvpr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zjdiiojy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3szoklorm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hmecfcng.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3riwfoytu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxnmdwzv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kiklrbks.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3iitvycci.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3grmhipui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ismyurcp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xosgycim.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tjsxkghz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3neuzjaub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tehlsaxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wxoyruhv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hwtpjkul.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3talxheon.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kibcvhhr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fywjuvec.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oceagvky.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3spwfusih.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ikobyiij.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3glychcsw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulehujym.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mavhsdhf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bazkubmn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aktcuwiw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wgfgbvlt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lphmqoqj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zelmkina.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3oavcmgum.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zcinjzhy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3illmzjam.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ihjrsqzg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pfbqdxmw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfctstp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ftjkonco.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jijnipxv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3enwwjiaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tszangya.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fjyspxpb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xlfdppgo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gajyxjbp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3eiiskrhb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3enuhutif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xoodpect.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhiiyyyu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agwjiiym.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgkeuve.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eoieluhz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xjlqvafv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ntisayyi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wjsswhml.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xwvvriya.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rtmledlo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ohrngyfr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bouzkkug.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vhlwmzyz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oxilyfri.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3modngmje.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pfjkstsu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bcodbugn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbkxbdyp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ytdbmwlp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kmrikjek.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mtwszbpu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kbpgnnih.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oftagwua.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gndpbmeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikwfvpdq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3epvdxqyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jckonklf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ybefhmty.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3svxlkwyo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkskvre.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vqmopxov.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3szojyjue.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjzbntl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3usyftqdz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvuoqiuy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpayfxal.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3emepmpdn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yxdelyms.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqngjque.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbycbwoa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dtcrytdm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hkktnqfi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dmwwhaqp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mvpwekcn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dlchabws.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qzvzwdih.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ueqtfcvd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pntwyuxm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioltbswz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rohdsthh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zgzhypmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwihano.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3itzhvyad.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lxcjgrmt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xgnhfcdu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qhxnuood.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fxqbogpe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ossnfdew.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oenprrwj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hmwvkvbe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnizwulr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkcrfqw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tutfszgo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yxvdglor.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3umhrsszl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xwkufcco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rhldtqqr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3alpnwduk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kaxtlxrw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vxcbenqq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3htztndxm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tpfkfito.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tsceehlv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3olwymalm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3aqrszctk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqrydxkt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kluupznq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjudcqke.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zvussgpp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jvupqhzk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3viggzmmx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ndzjswdr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3obqozeme.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3imvpzujw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrdfdro.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3flungwgm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3poiacucq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kbnbwckz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qagibyvl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tpdizkms.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pqgzlkuw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ntiobxgc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3prxettgu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eqwfhxta.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xqvlcfsd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cnhfcdir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qhefctru.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eeecrprk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3phaxsmiy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mygcjcyw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjufoax.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aroqztax.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eoqfslkv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3phlkoorp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lriitfki.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3skqvlobt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crwdlmxv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcybrts.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mgelccfh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rpvkaent.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kftxmseq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cdxhuxeo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ljmugban.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uhicpbgj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gdaxdpgz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fauaysgh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yvdyoboz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dudnzpfp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kezwcwqh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nbvycoop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3guvffrbu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3csglblrz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwxeayf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hqutnyep.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3demxfoiw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lmdzpyaj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lltzigfy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kchkgbgd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eyyqgjrj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3prtjrqhp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gntnugox.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ndsgqkui.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ajommonr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ckismnuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxrwbv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kwqwjywp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dyjhymtr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ypfcipsq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3izlgpxzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jnrnawvu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yyockfuv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mqzpulam.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vncvzbpp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vlhjtwhf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fuocxazi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3crcklcyg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xbkbytzb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dqmtsdap.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykbkuamm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvvwkdd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxlotbl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3essrbace.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pniwkqvx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kfnngkff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iypysmqc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3euzjchhx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mmvajfxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kwjizkpk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qlduxyhg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ohzrmlrt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yhhffskd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rijyojhy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3igulafrv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mwfwzpst.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uszpxtib.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3grdfcqzx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bdjsipqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iprdxsbd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fegwyyfa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygmxvqag.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cczzpdyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqdmrkna.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vtaopsuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arkxguap.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bpjvzhvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3idfqlbdn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wocoxubz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ameepvjg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rgxlojua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xvdbadzu.html


<!-- 参考信息 -->