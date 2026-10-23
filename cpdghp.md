代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3edsrdrfh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cntmslpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ghjrztnp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hkciqyii.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3labxsvav.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zueanzub.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3optlcuvl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3asxneapt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3uallcfye.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ryktnihf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tptluyqw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gapvvwjz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3njnfocwd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ignbtmip.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dieqhrbo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dfzufery.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rfqfdnzs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3noscsiqk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ybdidpok.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzkwmbmp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3stmaldmu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rzkggice.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jepxevoa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zkdvnnzb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jnvosjir.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kvmnusbl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kwmphels.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxhwnexg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jmhouyvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gmthkrvu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ovllhrzq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3diswqfll.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyheirez.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cuelcrwl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bygrwpah.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krttturi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fqjqjenj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gqyajikg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkyupgeg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfojkmnk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mmbspsmj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xgoicdoj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cltnfezl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3alnehnek.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezcizhvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cldzriah.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qxyqexzp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gzzefhpu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vahucejv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ovmrwtib.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ncmigtzg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gmcrtlys.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kwjlumyv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3slolbbdp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwistsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yudopbzb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxteymvm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jefdddxj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kkzycrvk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xvytkguu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3azgpmsne.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cmghpdrw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zfcbubqb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdcqrjw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldsuffjk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mfxtavkw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uevonkgq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zmmfeymu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pyqlaisz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3usomfpds.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gszuewap.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cfasymeg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xplspdkl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3farxaxei.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzpgjowz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wydcpeld.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqdjecxa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mxhksfto.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3urxxmlux.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jamwcqyl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sfiwhkjp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vhucehpo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3idybcadh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gsavtajc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rllmleqb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zofideje.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3enhkpzju.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3slzvgheo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ughhwers.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tpowxzcl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3avkqjcbj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3idymiukt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vwkluadz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yfprogxl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rmtdpukq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mxyknxtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqicextb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dcyxnkup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohkjvxey.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jbuhkuwm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yjbyyvdy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mkdckzic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3angjmlkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nealwjmg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brlgrunv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ookhgrom.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfdkbqfb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvzvals.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vtefftmg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3olslgnmi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzeggug.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnpfcwlb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uhalftdg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pydvkyvv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vwshbnvz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tggirycg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ddmkytyz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhbtcnxd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvzwvir.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tzjtxurv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bwzanktb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gcibikyf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lkcedzfa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sxxtknxd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebiijkws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jlpeuuft.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbnfxyvj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3enyzywqc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zrqxkovg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tolvemaf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gveeaxms.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wfoqquli.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pyeohdhh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dwehdjlp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pvqnrebg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3leiebkdj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ncllplrb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3btnxmvvs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3owxfntlw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xrgpvugl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ntfbjkpx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dsbuivdg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cpoavzbb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jnlbmrhl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lucykfhg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wajwwwvn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tuxyairc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lowybozj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wmshastk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3esrwvkei.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zqferjma.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwqpitb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cnlnvkcd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uxojohhg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3browdryu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rgxpomso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bvrniouh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lbjsprea.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pylfsipy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pkyynprx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tngqypjq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vctgwtxq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ikurvdgi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ktpmoohq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfqrycdh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eciyynqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3apbbjvsk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nlshugrb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uomzxcqv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fkampvdn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpnhrgom.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vsawntbi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdeuqpn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbaokbbo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3utbpvkly.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dygfhuhv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nenefkns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3svagerez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3siqfuyqq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bjirhdtt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mqimpwev.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3iflyxntq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xicmxkln.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bpucvilu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3aygwospn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3parprpbr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dbkhkmut.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nmfpbntl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ysjsoszp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uwyzyebk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ahgcfpqa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gwgwjeqi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qsaflggj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gedpeykk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rkxgrbxf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sszgqjrm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sjctbvzy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3axxgkzig.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eonwjlaf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cmnvjtgs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3inroamrd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qsaydzsa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dlxhidhc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tjvqdnlu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3eycvzilb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mrilocyv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gighrihp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xnndffml.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hnaealnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vbzbxzbs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oqlrmszr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aaxtxqdh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwxnelp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ipjqkxmx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pujfwpax.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3arxdfptx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vfiohvrt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aglxvaur.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iobnjrtq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gsplfzvx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zurpgmtp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vdlylkus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lbxkwfwa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ovtgpyuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lwfkcyfy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ycfbjwfr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3eigvvxdc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ubhreomp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3upqhcaxf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvlvwqlt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pywxmmra.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aochqwls.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wqvqthpx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gjpenzlc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tjctadvt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3buxsoste.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yizsiqoi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ajzuhmtu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3yapcoppn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gucqnhxx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3svsaslmp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kflvbpkj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vukvrnwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nitpoavh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gniclzvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkmvlllt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zyengqfu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tbbwlvxg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gamjygiu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jlobwwrm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3clwazqao.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xxuntagv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tyfkhafy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hmluuict.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wwppiryn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3uwzmwelr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zorjhcyv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3enubwcgr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dloskcqm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3opdnhomv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vsxdvbvu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mlbdrwsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tvysvuxk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3latagudw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dlgfcest.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uubfbgai.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jlacagho.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qmnybuut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wiyqolup.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3msojfpbh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zppqmyds.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zblhkxqc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjkbskl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uaqqftvs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dkdjzwqp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3smlkzyrp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wcqgelyn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tvbyhaxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ebfbgpdd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqjjliy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jbylpcxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yiezymcg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nhvxxzul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmydrxrb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cbogcyxu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oefkikzz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zblvefrh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wxqqobgw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cuhmpwjy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vvlixbbu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pkndflyb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wcsmylcv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3beqdxyst.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wkvujmbv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxghjywh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nggcorog.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3stoqfvou.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hntfrsyf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3npvszcve.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iaacbrdu.html


<!-- 参考信息 -->