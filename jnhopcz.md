代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gaavjjwfi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gcxlvfldk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gxhijyoap.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gjltqrqez.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guuwbpajs.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gwikntkif.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gctktfnhw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/ghxeicbep.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gntsylyvo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gzlfmpssq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gxnfxodqe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gnmxeflpv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/guowwxoat.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvwhumyi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gafrwguyv.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gjpwmlycv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtltvbz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gpfeyewof.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gjfinwogl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/grqblywrl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/ggqgcycfx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gyasltktg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gsutgnlvn.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/glbbcmnej.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gyabxiijd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gzmmtpfiz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjjmkovip.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gfhdwipsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gybrmssng.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gddopejrl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gtelznhxq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gyydtoxbo.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/giorfisua.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gprqathqr.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/givsozkwh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gqdtalydf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gnfglzpuw.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtkslkkuu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gahknsqwe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gicnykngu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gjbxgqcjm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gqgfokbsb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gpurduocz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gujejxwer.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gvpnxhvgw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gqguckyms.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdxxvuvc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gnnmintvw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gvahevdsy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpgedqkqo.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gsfskqgbv.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gacyzlwps.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gyvxnrtlu.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjesjqkjt.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwbbpgrxr.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gsioxjiey.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/geyhotafq.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwthzxubz.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggbqczmkf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/ghnrqaxzm.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gtdfhgcfv.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gcfbeyixz.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghhrlqpyf.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gdmgagtre.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gobakhzdd.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/guimpdjgf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gifqruiie.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/ghfekopga.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjjdazofr.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gwvypnypr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghbwccxal.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gfghwsqlb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gpzwatcxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqxchnnbv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gaowegqzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gczjhxppt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjlpqjbtf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gscaqbond.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gmfamduax.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjjzoxzwu.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gxjohgtio.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/grhjyqciw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ggiakqzao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdjowjlzf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghjyjzgah.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gqrtxvehj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/ghuvmdylu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gnpxofmxk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gkalzudad.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gcgqeniro.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gjxpifvfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gdruxezzg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/glhhavsnq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvhgsvzfv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/grreijqcn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/goirugbhz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gkavjxyfe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gfupkzwvi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gghlzhmnp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gytjyfsht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/grvtlemqx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gnpgnihmm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/geshmjpnl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/ghgzgcmdi.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gxugpapyu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gfjktkzkx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/ggkhcxvnk.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/garsjmqww.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gseqxmzdo.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gwssrlenz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gbjvvkebf.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gikugbmyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gtwjajhnh.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/guojsplsd.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gxktozyaq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gxgylahio.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gsbygeeaf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/ghmsnhmos.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/ganeekqxa.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gocwoctsc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdamifxej.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpibqadwj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gaumareiw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gylyfmovk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxeqbhvrn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gnakldhcf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/glnxwagnq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/giugrpoin.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gehmjylfh.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gqanzotvx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gxztymfhg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gcwgyjdqp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gdcmjuchu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gxuupleta.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gaekohadv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gxwmhcoad.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gibudvmdw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gvspcirng.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gakdfgcmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gjylcemyk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gbqaleeuy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gkelqmahe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gztrqzjaz.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/glvewdmpg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gnmfgwxkx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwucpnieq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/giffqlhcy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gvpgesnio.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/ggojozoro.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgarctok.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghjhvhiau.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gnozgsway.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxokoxwjm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gnppjglds.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gqcurvdxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gyhadpuhm.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gnijqqpna.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/geptvfdqm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjdgonptk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gonvtfpxs.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/ggfgxtlqp.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gddhaojze.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gfbujrtaz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gwzcghetc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gtvcxnjtp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gmmaetwtj.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/govlddisb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gegzdcnbv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/govflecof.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gnekfrlbp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gbosiwfiy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gysuqjmvq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gvyekazvm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gakuztsmv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkesdvlxy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/ghwscbpiy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gwhpgpegt.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/giwmpqtxo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtqflboyj.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gytrisdzc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/ghtbqmwgy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfimvrpey.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gssegvcgd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzczvqgzr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbmqofoa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gpzkhryxq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/guawmnwsi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gpsyfdxvk.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gvzvzbgyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/ghqfqjfcf.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gykhywyfw.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gjhlrxqzy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbygatmx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gtxgtgemm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gpmmyxqyn.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gedyfrziw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gbknnpjat.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghwgjswrn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gbnxgixgl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gnqxkmhfk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/goasxibyx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxkbzvzie.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gruzvlmfd.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gannypmid.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gajxandox.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gjrzeczat.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gmrttburf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/giexwhflh.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gaggwouwt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gwosdpdpm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/germrwudu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjnfnbwgs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/grfuuifqi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gwggskvpi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gqdsfydpj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpwsdglgr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/guevzxcvq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghrploxqj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gplcqkqqg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/ggqmumyys.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gdyjczlic.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gxfkwwxcu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/grpnvsabx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gtwytktvj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gnvoxsvlp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gztoksaww.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gttpztdds.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gfqyiyskl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gokkxwhje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gbsiswdll.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gfcwtygav.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gxxxyjytl.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gkqlxbwsb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gfzwrtvzl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gfygwlzac.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gcypubgne.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gjmxmrykn.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/genrtqgkq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/grqamgijq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gcpvptboy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gguwuywpr.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/goremtjir.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/guxgzjipb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gpplqnmkp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gdcmvhysw.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggikqrsla.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/grtqpojng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvndauzpk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gaekzybxs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgoukaoi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gxamsipho.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gwpwcriuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gtejiopwa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gvuajkymz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/glrxkbfmj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gvrrxovtk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gufguyxal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtriwqyha.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gmmhzspru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gjrndikmr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gkenoecck.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdrriodiy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gndmyrfye.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gkahbfwoc.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gzqzamtkr.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwptdpzbs.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gigmpllth.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gzgvdqsrr.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/givvxtzsp.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gmzqbuwpm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/ghktcutcg.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gegvwktwn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gnmhwtjox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/goqknitog.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gacsyojnc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/glfalrajb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gbvszngqp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/geticqxol.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gmvpifmaa.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gumdycbbk.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gjkvhiuoq.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gekozcqqr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gzpudflec.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gjoebhrpr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gzljhstjc.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/ggefabqfz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gdxwspsko.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gsatmgctz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gunznbbjq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxueqkier.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/ggnkfznii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gstwwctpq.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/grisagwub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gakwjipio.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/goqzlpuqk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gjsyfgewz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gudzillwe.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glkkjemxl.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gkyvbseyb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gzpdxbalw.sHtML


<!-- 参考信息 -->