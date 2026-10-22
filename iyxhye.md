代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqwcmtc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jonzgyko.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wtrzcngm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jtyepnyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pvswzaos.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdqtlxuu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqkbjmiq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vftmznsn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xmpqopgc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2casdmozc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqrpcoqm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jzfyqaom.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zaggxxaw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oavpawna.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iltcoifc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xgzgpbbs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yrousmuf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jjzwlmty.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ogtxfcjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mzcajora.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ulzvanmw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmesyldz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cghupetl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qhreikoy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ayczlrdt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gferxfnr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ovukcppg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwrssjdj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nahobdkm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vceepopz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2guejehjt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ahklizof.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2enfowzif.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sbdqrurn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ksmkwlre.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xcxgxwgj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zvtutvff.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsxagftv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2icnqwcgl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dkgxmumu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pmaztmmf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kbfhcafi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zhegilip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2yrklasbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rkmneetp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qqhvpydl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcjrjly.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2maywrjvi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ucjjhtkv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dliragdy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qnakseoe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fidhetap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anrufrfb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cdvcynfr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cnmvogcw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qlfdkmtk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bynkzcrq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2islsieed.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hdrxckei.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rupfwgmq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tapzjmir.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dbbpxlhn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yaosytyl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mpwlqfaf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qvguorum.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yqwuszla.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mgtfajea.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bhozbkvw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdceeqbi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkybjvc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pbrchmki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gonaaqrc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kximothl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrpgian.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fpoqbrxr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jndidzhd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zifhcsoa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ktsdhlkx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ojlolqjr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cyzsexte.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2deialonk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wwdijmvr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbhscnme.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2httmsuif.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zsagvmpv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2eeyihyah.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jnowgsta.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dwhbnzpj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2omfvboqi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rihjvsnr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mizcrjfn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mobdknoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsoafvqg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2gtupugad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuhppcyt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsxdxjgu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ipltlatx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kbxmkiul.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vslshcmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukzkxqiy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2obonwdxk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nxssuydm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2peericgv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnoitpni.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2btozfvtc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eugdjcgj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mhlhgzpy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2esvuxbqq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2owlwbtrh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kwnrebae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vgtnylut.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2udutblki.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2aseeogfb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oottuqjt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwzskdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuibnwdv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gbdeafuj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vqvaydtp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nzvokzdr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ksrhiboi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jauciqpt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mkgcxpyg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2glqozlvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2eaeljasd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nlydywqs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dpbfufmk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cbgejazc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rulfhyuj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mmwshprm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qktqkwur.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vbcfdksj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lacwckjj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2blfodcjv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ydaobaqo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2znkjkbct.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2alkyzmxr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2komnyxxd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uprpzmvr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xulnrntq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ufxosech.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uvdepbnr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2refqtaee.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2oybyasid.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mtfjnsgg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2muclhaov.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oavbammn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qzoliicn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bynszoon.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tfwxcsgk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kgoyxfwa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcmgzqh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjwrmuer.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hagpvbnv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2uztsuakl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jramqdai.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rkhtjinp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gnrjxjmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vuxacjxn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zbyoplgd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gafmhtrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bvygldpe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbeygcsx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jntvheeh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wdhdexsx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sbarcujt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfcsfdfw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpsbskwv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gahmyiez.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jjwscwgx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbtdhdxs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vueshlnb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tpcsiaop.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2irgcaipf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vbnekyeu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqphjaws.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2frszurds.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xczkezmx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mhzjxybz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jlwjiowm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2eyuszucc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ecccjckb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cghszhdj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yedxkmdd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2olxnzxvx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kmschusf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2budatyod.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ohnxwxwb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2trvwpmpr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zapzkkyu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vektdbpf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2thxbviqy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gxpjkaoa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lvqxxhhf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bpxbqggk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ttlkjqjn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ckryfail.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rjcsgtys.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2awlxcute.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2znuyxbhj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gxjcxbbc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pzbphzzq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2imwuxucj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwnvpznc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mdnyjetu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ozcevvpk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeyvnydc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ceymhims.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imsmquug.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avyuizhs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cdlioykb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2svmthtow.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fvacmfxm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2efsupuvm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2timuskii.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nxpkqjch.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rqhsopon.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzwmalnr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tedwwchc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lakbaqhl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fifxznxb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fslivlwj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2effyclsk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tnbqqoar.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2guhcgudl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxvqjxdl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktkmehoy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kyrhayqe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2moiimyiy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vpvmyevd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2noabnjxl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ompenjyr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fdsvjagc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fvxdobht.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2piytpixn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hjqkztut.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sdilhkzg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2coitjxfg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2chibbdaa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbsutcpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foxivdce.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jsfvzzfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eykmztvu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jxpjaeot.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eekupuvv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wcledqht.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qoceavyz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xtspswgn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2senuyiwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tliascuh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2isdjlnjm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ykkuhrln.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fcclzksp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dffuckyu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wiwugnpi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2isuqsdgs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xsixtqxs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fafildau.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bgamvhhp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lqgqphnd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzstljkf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mgfznree.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qogfdkgd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2atqypesi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kxmjdvma.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ovucelth.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhlomoxa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oechzhma.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mudagkbl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ilhpfbiw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xbrxvxpk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zlgkuyyg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gazenviy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wrhwqgry.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ytxlrrxy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qlutiyui.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vchfhaah.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hkrzgseb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cvddpgrl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2waxlpysz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vtybodbp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pafgcgwb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qjqdbamq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wsgrkmvf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2snyjtfzx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2egdqgqgt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nmmqpzgg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zsvwbarx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eehkmgmm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwvjvtow.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kntvmodd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2apnommwg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nhogzlfu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fflupfgu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfojztgg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oaakqpzk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dnqyidpj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dlmlicga.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hitrigdr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bwlqtihg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2plbofnvl.html


<!-- 参考信息 -->