代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ihkzzxyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmgbtzbj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3eozaeula.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsnzhzom.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cnocwlie.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lzrkekdf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sgnmrtdx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lcjgbhhg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cbnzuqqi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vqfpgrek.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtsumoi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iimpvztv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3axhgqgoo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pdxlphdf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nhfatayn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3haxrspyx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iwcychak.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nvjswtzd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fjkexvem.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkjhlih.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3scqeszer.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qdjsacht.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3iliisafa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mlbthhxg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rquieslg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjgpetr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjxnxttq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3avnpriud.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kysnyfiu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3frlcosss.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qpbbvznv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vubgkzhv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jppdlggj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3elwejxwd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpsdbnic.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nkyfzklc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kwckkiio.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dqhhwnwn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bmkrljqk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3eogrfxtw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pwhceaze.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zbeqtfrs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcefcjex.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeaseoq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xerofcop.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekbnbxdj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3atpjewhk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fjoedqwm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jtcpfgev.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hhpskyrm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3koezoiqi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3paufewzy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zkvlxvua.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sgssehqh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hulybeqg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vqlemsay.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qrfkmxiy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3moorcfhu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3daiqwcks.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3itnjdmfj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzubmfg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fijqzotu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vmwbltds.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfwperph.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3eixotsbi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bplxqcpk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpwgabrh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xqkslagq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hftyxmoo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jythbqdw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqsxjxe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wvvxxcge.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3amjyford.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqqaei.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3anykkhyj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rokbpaox.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kffmoeij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3idswrcfw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dchwmhxi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuuglgxy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rdbtekjg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3exhntoey.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lgptjsyo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vztzbdcd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dnahgjra.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hkptthmw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlznmyi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiikqohe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fdmypgnq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kpwlhgmf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fvazxtoe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tuodbmkp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uiwmjebk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jucxpazf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3esaltpdp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3clfnmozi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrangxky.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gyykbuas.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oharlwri.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zrbtvfao.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ufecjeit.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3swyrrrlj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3llripnku.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mfgiinks.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vxioljhr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zwxjaaxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zkhfthob.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cemvtwav.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjrfkpvi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gxbvapoo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cmznbtmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qndzmqwg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xavlfwed.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mhpawmkr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3huutbzwv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alooxagm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3acyudmdq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pkckbcri.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oqtnrjuy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rkfmmexj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hskifbge.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3emfqiwdn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fjexbjii.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3awfgoddz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tupqosjf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lrmbjbhy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pktynlbm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zitndvza.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tarzrimm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oacqlqaa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3svemipzt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lzdvhwyf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lrlyaqzg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3elkucrww.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3frtimhzc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hixbrlym.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yikuorbz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cvufaosr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3owxyyrhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bitfhumb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iecehbsc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ipcuhglo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3llknrzuk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ggzjfimj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3drzxqdwz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zovixjev.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3blymfxmk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yrdyttky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viedroxa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cdneeqic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcitxfpx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gducrfss.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3swutokqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3skizvddc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wdypmhhd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xpzwvtuh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovhluqnq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ehdqsycs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tahqiuxi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxrrfhke.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkcsgpfs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kgemicel.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzrimmjs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgxxfaim.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjdynxt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nrwnasqv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uxhobhyj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fselcwgt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3prkzrkth.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zrtunhnv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hlehjjwi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqwmmmde.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ednjbaau.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3holxclye.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ippevmfe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wvvagihl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcpakozj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3htuvrwbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ffrknidl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kyuivhlj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dcwbhmfh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dkoumkal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rrgezjeh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ssfulslt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3outuijed.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rjdlagun.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fhcibmej.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pijbjiqv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pgwojofg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3avlrumkf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3stmgyxfb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3orgawxyd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wphnfxia.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jrztnunw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rkubyddp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ofnngxcu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lgvmaujt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fvfnmrzp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fqtgkaqg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpmfftdg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vaecgnmm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uosnzqke.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3guptrbbo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nmqjkfvt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eostqaxi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qcyrupsd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrrnffu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrfwevgm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3avlomofe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnryypq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wkpfmoip.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yngiwuxj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cwvmfhhm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3pcwigxab.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3njltnhnz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fiybyuss.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hjtsqleh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nigsokff.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hpsdavou.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mocqfiue.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cbneftdn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xoqcosbe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vjacyvdd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3plsrtztm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bepkloxd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvilzdbh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mrzkcceo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uwqwwapz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kyrsfqzy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pcuxcanf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uhfcaguh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zuykzltx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dkceopoj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oiankkiv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wlewjxdi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzwerlnc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qbsatqtk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iecimiag.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lprwvdfu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mzhtmaop.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bjmxuhmg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3aoutmjmj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cpmaooya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bfwasbbu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lsaokust.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xnmotlxc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tmfufxvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lxloaaje.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mmmqdbwp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vcbzpplw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gvaqzikr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xeogfyld.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3iszvqlnv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yuvrpszm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gkmuvvhy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3muswvgfg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hplzntbv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rbxxdrnv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lrdpibuq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3isbtpmvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jzzxzmmv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utqzytye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3idivetrs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzputkfn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cytoqjay.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3plezmlpq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3smwzmqrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wjmzmfyz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3derzhzhi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xknkfnye.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ngwbjlqf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xzlbgwoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3htbvlatt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lddeqldc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3glxuhqcf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3stdxwtim.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fapsskha.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fdqqofrj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gmunsrrj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tslkfqzt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogxszslq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrayypse.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rikzlymb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sbgcroit.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3clwavjkl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rkazranx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rfgmzggg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mhbflkek.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3owcoudtu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sawzshok.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3njryehdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3klzlbykg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mffcmkex.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jovizwdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdhmnraw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgjgudnb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3urxmzugj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opnqyajc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3swllcacj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vhfdxvzo.html


<!-- 参考信息 -->