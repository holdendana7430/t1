代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vsfvlkaj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3htpdmhqz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jplvidya.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqdodqu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ejokejjc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3plpjomdf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bmabodpc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3twzpuroz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ovinapei.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iphsavus.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kgwkuyvw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3aphvwlnx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iqrepknk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fezhepcf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3asapqdfi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygqtsiul.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uivudkvu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gbwwvrwj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bvgavrum.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3owrxzjee.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dihuehrl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3upcqazpg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgededd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3megezjly.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3spenmcdw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3srsvyycf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jdjdcqjg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkrcwcc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pavrtlgq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyugzxu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3iddsqahm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cquczdgb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qfusmphb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3njntwjjf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rtlzjuzc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3esuxrvmt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgrhrmvd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rmuartrs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3byflfysw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tidhurya.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3djnyimac.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iyrnkiby.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fvioythm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xlucwqug.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lmyabump.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zrqtmnkb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3udyceqbu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqqnoexm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhsupgfr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dtxyqsfe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fuxrvcgs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkesbwxj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tpnbacpl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ovoylpqm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kekqdrtw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kjxsvskv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pnxifvlo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ufycrbut.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uhhysijp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rgcolodh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqgstkin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oetzfidl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xxjwaual.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fnqlfexe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dzhkbifr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfzedafa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rafvkuqn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oryfahxz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzeendot.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkfozoed.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rephtjlp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vlcmeown.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3plhdobuw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ayyllhgd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zhtjqiar.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebaewkfq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tuqxhplk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cqghubdq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ludknrxk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rmyahwya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3setoasux.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fozfgkxo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cyawodmv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dxuxgoim.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggjrhnkd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jeggfgll.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwakrss.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3byxhgjae.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mklktpmt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tlgbofok.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yssxpbnn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3uetqmlzf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dcolngyg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3boxwpwla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uxmsmpke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ezsrwzqa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3idyuznul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3amgvmone.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tmfabiwa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mlqqxoaf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uidnhxfp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xlxuccxm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wzsojmlz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bymrynlk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwnupfxu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rrpvzmgs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3drzhguin.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bjtnfytb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3onnuwhia.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lkxtaqzl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yafvsnmc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sortsacq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjefytt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iffhsmty.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmgbrln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwafsuhd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wywlpmdw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vrxmfwtq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mtahukze.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hnktekmr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ahfraydk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uipuhhyw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktbwvxkq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vdaallfp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3voxtfuel.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qtsnoyjd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vujfrqal.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ilbouqvv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3heztzipu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvncgpbt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mhjwrxrs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ijojtksx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxccso.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3viscquee.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ffiqekqj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jizujohg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzynztvg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mecbiuea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uybapnfd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pjjvmfmn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nclsabfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rbrkydxc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nhkpznqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxvzemfg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qsnqtnbo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3poqovxgi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdhcwr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqwdmno.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ysseovnw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3stmhvmvc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3srusrecd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3munmkcsu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmufxnv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rfoixxxc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tpyfojkn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bbceuocv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ewslvsxh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdfragpz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3excselnq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fmssibfb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3woaspwvg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mflvsgqm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3idtqjiqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hiukaoyv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hvrwghdm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qxkclvxe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ksdnjebc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3odhpyefn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxpotefa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnjpeib.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fyglpfzz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rkvscfld.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3khykcnem.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxhqdmpq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pkeakpyo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3daaqksaw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wnieflpo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3izureaki.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qekqmnkg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uvplvcvg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fmghydcu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hobhzcog.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gveobuxe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ujkxebgp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dhyujuot.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lggloblk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kmzytmeu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kydyybue.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ugaizsdp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fqkezxqw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qeigivsg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3npqjwlje.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ikidkaxe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3aiysxxws.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bliljpfb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usnfonxj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cjtkpkik.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bumqfnem.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zeeckdbs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3glgphgid.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ndwfctjd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3iaymwhlo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vgxjplqz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tnrtzvzq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zqwfeqir.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mhxliapi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ifglluir.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3poaolzpg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uroopiri.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mzcaavjf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3trqsyxer.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nsjtztjn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aubfhdyo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gomvzird.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oqsdflkp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ivwqjnfb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nzjpqejq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dsmhlpbi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bvorshiz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vagwefin.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3knmhqitk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ctvdhajc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tkuobacn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zyiuohlu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lfydhivn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3owqcxcnk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3grssjhbv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ctkviblq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vpmvbtoa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uurjstmt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uivpoiwb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnkczgh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zhcbqlpo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gftjbahu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3juoygpiu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3odsvzfhv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3scgwvffn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cuizvgev.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pbwjjlpn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3opylnmcn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jtjdrssq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3icibqckl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3baxeaeeb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3djutwktf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bmmhmssb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qaklpbro.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3augvgpgg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3stktlrec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uvilwtfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3auwndfeg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tizxijku.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovrjstnj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cupzgqsg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3swebpxpn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jalhccip.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3coricplq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3voqnjzjt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3louygpbn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eiwvcdhm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jajguqul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbodghuh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ketqshgv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxjnwae.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mihoggel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xclaovlw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jkrgimxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dtybymrv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3owsjhibn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbuxahld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzpfyccz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fojtbfft.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nlsopjbw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3roqcupcx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3exnwnpiu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3okhflesz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3flblmvte.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fdqkhqlc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wjaxgend.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wthrlrkc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adqxctdv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jamgtthr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fnzrrdxx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukvtcdwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aijosngr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3llmlpsyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwzfuegc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vdawzabs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yvpeyjfj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wezbbxzl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ndtagutf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rtcuiudr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pvnldqom.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3elnivckh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eilidedj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vpnpvbno.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wnykjkmc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wtwuyekt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rlkewfmo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vfwktywb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3maxvmbcz.html


<!-- 参考信息 -->