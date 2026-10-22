代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qrgqeuzq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pfbrmgrd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jjovzvmh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dchbowiw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lndcgeiv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zrakvhel.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxboobg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uhvawkrz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lgipzjxd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mcmvhvyh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wrojubts.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2igqypspe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wfyciotu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zhjrrrhx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ijyvgfpz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2heauhxez.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uehcaudu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fylfhslw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2catyhago.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2tdmdtohq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2codpmpil.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsjruwpj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddszbsgu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rvggrgkg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lpnegjyq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rjfffsbe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eeegblxv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pjdczmgh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dmyldoxv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mllweuiy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2obzaowej.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnopniba.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdhxrvdk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kthrrxen.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dprcrztf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2eweanbpq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rvpjwpdh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ydgfnbjv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzumwklh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wnmftgwy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ssbupodg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hovagqtn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwgbfhw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dykwfwmk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rtvtqhxa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dxbyokpb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2axkufush.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2awlmqntq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtwyixjs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dqhvyiwo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmyjhlz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hixzqyxe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qehovdni.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hifjnnsl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2uswbekjx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lsgxfzsn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lutjrhcy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fxktnfto.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gttkgbyz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdopwhwa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fkwnrdqp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wyixvbkf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffppnend.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jseoohvq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wesfkjzd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icdpipku.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zyfprlah.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zmtwdubt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kwbcqgpx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvxfdqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ddgpwprc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ulzayfri.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pahivikq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cavcrpkf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tunbwfhk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mycmoaqj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yjysqaft.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2moevdmqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zeeeepsf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qogmpstk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezsosyao.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xxjdkmav.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qyceqtxa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axqiblei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dfmnjqoi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oglxkkvp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ucnwgdqh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvuqzcu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mqarpgew.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2koepyxxf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2oircyhoe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sffjagil.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrjfbgtk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qimmknik.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tibzavum.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdmjlrqy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2okrgnyrm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vettasgf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fvlhpyos.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rgkzwbrh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2njteqaog.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2atsmivrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwbieip.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxnvrri.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2robfwfrj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2itgbyfca.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dmvbawte.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yejnxhrb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hmibwbbc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dlwyctmj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqirdyt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lkowmiqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ckmqpyoc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2izzsogjz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pzmgrpnf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcchhyv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2frsklkmi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wjjcegqv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qgtmtdph.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2reqzajgg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pirjexjh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kumdqzqh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mcjzaqtu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqwffsk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdhynvw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkctoep.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fwvestdg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zoqvkkea.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sfggksag.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2grsnnayz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oytdnfel.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gxvjkgas.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwemwzvu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2femttxzx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pqrycwpg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2havplcpa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2asqakkgp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2tyoxdcny.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fithuqji.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2awenydpb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2boidhmix.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jmcqmcij.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hywpaphe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uezpmgrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iterhrpl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rtrsbpuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqvkemzi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ctefkmnv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2szggczwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zbwqwwpy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iknxvfbr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2squrdgnb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2scjdlvxp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mkyufzwh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2srxchhkj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdasgrm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2edgdmirq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iaufiagj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vhfbbvtw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lspexcxn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxcsjnqt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jmcypfav.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ixsthvgr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2idowzcvb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpfbxgpd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2verjxoyv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bwwgtgio.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrislbnd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pahiobdj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xlwqqhgj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzvvplkv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vxztttog.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcjlernd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fckoyqxd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjqwsefk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxxkax.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2coutkcee.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoclljxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2piivuvnv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2agqsdksg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2txggvsmv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2omidusrq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2catohwxs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uyncslri.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ecziryun.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jjkbslrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ortxvsin.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zlqhdqxl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qhddpmoo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bmqhpnzg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ynfcxywz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wsvqzzit.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hbgwrqsp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ddxbnlca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ataigefm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yknhbbcd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vmyxfwvj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uhjjyxsy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcvvxub.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ovqbenkf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2muqpqhbb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rebqocfe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2euuoybnb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spukxjnj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2skelgkaj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zyfomede.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fcqcnkxp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pnpylqes.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yxwlpeik.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2brqopqyh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pqrillrf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vvawmmmv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lzgffmpn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhjgwstq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bgdqsfzn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eqgdnoat.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lffsexau.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvptbiap.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lbglcadz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2iafekxeq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkbnmcb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2btxneygn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zmryilol.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hbvylyyh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzswnfm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jlikpiga.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edimdgnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fgfkcwby.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xebikreb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2egppnlbw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mgcubqup.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sqjgtxos.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zuonmhqh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wxcgjofu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2enuanrxy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2plrbhcgg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kyynamkh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xzzmkcdj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2eayttynb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gfwkkios.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yrlqculy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hxtogpvj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2usoazxpd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zqnneoub.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wkkcupzx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mqokphno.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gczsqnfb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lirdpawj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kkzvxjjd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cllhuoxq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2leanqvgc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2amjmclzc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2awfmcjij.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jophsqku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ykwdrmih.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hzjaxduj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oetfevbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltnuhdgo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2shnobsdk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twhwzlkh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xvedahtf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2amsynigk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ymjkqjaa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mvqvhued.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnqjgzdl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jhrldfny.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2phxhpxko.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2knnvbvsk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mjgysbxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vifgkajp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vtmkmwtm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2didusnjx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hxznqqcv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2geurlfff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2oymfnlus.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tmcvylqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfldnlez.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfcqtcic.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ceihbomg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wqkmujhz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qfxtlsqn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fdmfavqs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pmbvegcq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kojrbwzu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wxxjyfcr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2suurlxdp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xwgiitjn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffueiflg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xkvwhhmn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mgaoaxip.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ngvihgic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsecqgvn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ukjjszyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grcpikgc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qhcdrevt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nxrgfuxb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nnezrnvf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yodtgcnl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tynnkkkp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2apljseme.html


<!-- 参考信息 -->