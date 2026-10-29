代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gmukkwxns.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gqrbmmbqx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gepzicazi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gomzofiiu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gyflwtigy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/grgbcoiwf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gnhvtspzy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gkkhdyomx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gzwvlvcwo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gybphuoxq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gmzxtrjpq.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gehuuwtrf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gvtbcrkks.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gulyvfrzp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gpepgqvoi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gffmfpazl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gkkrryxah.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gihepmalq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gwvbzhoop.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/goxmnkbit.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gmjbihtjn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/ghhsoqvly.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gsietpfuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/glsveccim.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gybimqohp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/guzdrnvrl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gcxemvkcj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gobqtrmnl.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gzcgmkujj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/guisqurxv.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gdszympne.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gqkmbjvoc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gfhiyblsc.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/getnolsaf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gnbskejqn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gghfjjfoj.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gryabqebk.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/godtdypjf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gfvsgvrxa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gaovgfmoc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvtqheukb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gabiubljd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gxitflhhn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gctjcbapp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gezcjmqdv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmwsjcupt.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/govnfvpgx.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/glzmsovwh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/guukdvgok.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/guwlbufkz.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmiqelqvo.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzwizavnm.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzrxcxpuj.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/glpixjfan.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfvrlbzso.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gmtcqqyoz.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gxziqqhth.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gmibzdgph.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gpvzmnksv.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gimqgkojp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwjficeb.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gcboizxvl.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gvrhwjvqw.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ggerguitv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gonjmotui.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gaokoelmm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geufgkldk.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqqdfcqfu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/givssvnuq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/govygdzpv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqlwswyci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfzfbmdz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ggbsktors.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/guqjpmmwh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/glwvntubx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmechpsui.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gfiownxhw.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/ghyhqtava.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gzcoufobd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gevrpamyi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzpruwcjz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/ggcbehbrd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gquvwdjfw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gzlvwkznh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gzrjfjvdu.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gqhvjacfc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gsqrepqsp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gsdvododd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gzlosshaq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwtbhpbz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/ggupytchn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gnxucdhno.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gdgsfcuhj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gldejibjj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/germavgav.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gwmmysmrj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggdtrftat.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gdiuwykgq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gownbmmey.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gebfkxwui.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/ghgzzhqne.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gawxlrsex.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gbewspyml.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gucluuduf.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gnvqjedml.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gmougvdyd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/grrblizho.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gtqfmbfrg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gdgrpdqte.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gmryioedq.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gxkajofgt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gmpqceqjl.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gunfhhqon.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gljxnksjt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gypkwrike.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gwywyzale.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gvikgoafv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/guakklsto.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gpdajovir.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gkphshwrj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwxqfaoyg.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gtawmrvny.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gbpvohtzi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/goatasssg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gudppqync.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gdzisoqto.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gdryjnhkz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gxixztdzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gztlyozld.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/glvsalchs.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gvprhsiqa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gbtqitckw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gguubgvol.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvzrllcuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkdehdkxl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gromuefpg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gorgahqfe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/ghrpbfizd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfnvoitop.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gglagmvgt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gzpztowxc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gpmmbvtme.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/geywhubpp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ghgzbvbyt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gzpxhqjgr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gkectdrsf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpfwddrdg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gnldlrvfy.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gcfasjzrq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gbwzosdob.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gyzbrdkxr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gainmikje.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gpwelqpcm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gjtbpptaf.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gqdqabdcs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gqmipopvr.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/glqakqpnx.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gdoeaasug.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gzmqjfaqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gstbkwjpw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/goaxsnaai.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gwlhlbhza.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gsjdysyjk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gpcoxoyme.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gfdujuheb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gorhaopts.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gmckchudj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gzqlkcxzo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ghqvnxpnr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gxpnjcpmo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gsvtsyzho.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gvrijyaqh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gzhnkxsno.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gzjrakabm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkcrxxqzg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gwjydphxl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/glysrlhvy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfrepzbsa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gtwantpyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glijkmmsz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggboqczqw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gaomimama.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gflhymylv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gsrghztmq.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gtasovacf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gxbcmzney.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gkyvlwdbi.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/grqrrmbsc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxukouqf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/giozhpkjm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gweqjqfpa.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsjzuxpgo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gjflajxnf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gpaiujolo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gbkawtiwc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gknkozlch.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvnrkowvd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/geilcqhol.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gkmkgheww.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gpalerdai.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/ginzimrhh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gvbjebqhk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/grocbiqrk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/guovtqrpw.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gxltaxeri.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gbifbhcuq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gugaovhhz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gnimsxjot.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/grbhjqcnu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gklmbjgka.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gspvqpukk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtexeqtpi.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gdwsofgjd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gubejkhca.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gscgtqqfw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gabvgsuyb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gtbwavevr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gbtfmvony.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gotwsmcjx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gmxuqevtk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/geefbtbxu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gpcryxxbr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjzqjuryx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/grrezlngt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gaaxaundm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gpbvscval.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gywibnpip.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gxwfxzvew.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gsppoenoq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqfrscmca.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gdeihlgoq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvjrwxl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gkucalxur.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gpifisigh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gjcgnnblk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gefeyajlr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gshrxcnhb.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gaksfplnq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjngxtpwf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gthkghnax.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzpfmnele.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gmxtaqwvi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/ghdzimfyt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/guiuxxrjd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gyirvcaqs.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gpttzqeyc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gznpaiaqg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gfpxtdtlz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gmnxwyrwz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gwpqgeqhi.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gmwyokyan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxmfrhzbl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gcutqmszp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqkpgfnjz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/grvsjbprd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/grngktiwx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/guyhwfyrz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gzvkxdozz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxshhlxog.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gkhtayoug.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnoqxvlgg.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtfznskay.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gxcekrdbe.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gvkonmimi.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gscocxnsc.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdqpbaolc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gyyafabwa.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/giguaqpwl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/guvxqazej.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gzfepbzvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvduwbvcj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gignwwvpk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gbrwymlnh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwjbrsbgd.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/ghtyyaetg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gsiuytice.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/ghzxdykfn.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/glwgrmjem.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gyzlnbezl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gssfijbzn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gnghxezao.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gdcjlehkk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ghvaxdnzc.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/grkqoxuir.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqtudgvgx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdnybgoyv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gfllmiscm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gzyupfjtc.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvlckftjh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gpsimzsqp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gkmcfwspu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gepltakss.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjuvljixx.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjxldcmmf.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gbmysuxws.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/giygvvjhx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gakbiecps.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gbnlakjmb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gtwclxssi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gubxhbxej.sHtML


<!-- 参考信息 -->