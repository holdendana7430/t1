代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gvnnzhcwb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnayzutc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gugpoiimj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvmijgcl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznoorxnn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgtudcbv.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gpzelocpa.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/gfqsloayi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzqzebj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggksdwygq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhrjwgrz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbkjouvd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaosevhi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gstkpksrl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoxkkcmx.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpttvogmy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhgwlvz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbhxhyup.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumvnavbk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/glizfeamp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywlrnrfr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwravvc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gjfajxbgz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gddlcqxjy.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuycjouo.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gaaeljtfw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghydzlqrn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glznzyreu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagoeuejm.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gqhdtbbbe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoebamaj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzepcpvdw.sHtML

C#:   x is int or double or decimal
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqgqcyi.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gnocmxbcu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpocicxfm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqwuixfp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glekoctmi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwhvvosj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgdxxrzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmytpmkw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnktvjzt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmxwtrz.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gfepyftjz.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjszqxljo.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsgvkhej.sHtML

JS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gmjeydcns.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbhiftyf.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grejnkuor.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gidcfnayf.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnmyvqi.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsrxwjla.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gemxkjsud.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gsyxjvvdo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glngpssuq.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvnoiqti.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gndsnpgbn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztkcnul.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgletixc.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnmmxlhm.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrsftii.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgtbcxxy.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glemlflte.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdfswqtyy.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/goknmgyvm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgcbypae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gesdnmibg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrmqqcbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxnqjhf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxuehyxw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvchqgebi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcfsgzp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecwbqddu.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glkoqhnus.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmqnrpnq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckpiqwdp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewhjbdph.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvqzcpnuc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdmnhwa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goovzblyx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gojouiulv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyboiqo.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczfmfro.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gagvmumkf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grcdjrwpm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyjgknjq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxitflb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fanxiaobao.xyz/Article/details/glxcaahtu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gqvdcpped.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufidmtjt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrtacoil.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqwxchkv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gusndhriz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbogzzvbp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoowlhza.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/grvqxodri.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotxrnkoy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowcsjpb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbslskgm.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gviilzyuv.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gsubjvgmt.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqubwvtp.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfiwaoe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqqvwlto.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gaxzferio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gaomprimo.sHtML

Go:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gapljvqpj.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhdgmejv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gbqrjnuoq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjclvxvz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxnnttoe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjfvgtqo.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdihzpfs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlizdjmf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjccfecd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/grnlqmoep.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssnjgjzo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gqypxkdti.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gpdlqqluz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gmupjdqmw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gqsrpeipm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/ghixoaxpk.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrnaifip.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gljwyvykh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwezewlz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckbpjbxe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxipnprar.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gzsrdcjat.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftadlvwm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gseizdyue.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjtkbvcq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gucrnebzi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gqnlsokqd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmevepox.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/goggcyvkx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtyjbimac.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/getlebwlp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevptkwf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbemploeb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiygrkce.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gruiglvwg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijglzxnv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gxxkfxnbq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gycczonea.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjdixqm.sHtML

[C10] 变量作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdlirjgr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/gnwnoidxy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbrwvdcm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gqltzgsnq.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfadcrpzf.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/grfxoxtrf.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gbnekbjmk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxuneyzv.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnkythyl.sHtML

[C11] 模块导入与导出
来源：http://blog.fanxiaobao.xyz/Article/details/guyztnfbz.sHtML

Py:   from module import func
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqnwllnt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fanxiaobao.xyz/Article/details/gcekwsckc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnzxubvi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrfyfafu.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxrktccx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gddlnyhhz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxaoajv.sHtML

C#:   using System.Text;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkcjonws.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gbremouwn.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/giqdicwsa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/guydipjxm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpgdbxo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gogwtnotm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/gbkadllwe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gehafftcq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gxtkspuin.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidwfehaw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdqyhpgj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gdkwlkhor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwivkelfn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmicqfrez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpuyaizg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxoxtjbs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfntvfxc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtyiagu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsonueet.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhpcfnv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrozwhg.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gczxqagxa.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhkudnme.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqimxbqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsvsiss.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthniitfh.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsmramss.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/guepfecpq.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfsbazs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdvpzxb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gckrjvzjn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxpmtcsk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gflzglisd.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gbcrkuadt.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnegtfaq.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimucvyyk.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtavfknii.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtduzliq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gadecbcuv.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gyidwbcdg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/griebrhuh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/gacsqgsbh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzahjcjv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqerspml.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gigpibeee.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsqczswz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmkhmhlz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpedqxrhy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/godfpoycx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrgakxgw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gudwqqhzt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/ggyxjowde.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gulcxgpsx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gncrpwwal.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/geoaeopiz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvemuydag.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkngfiml.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvorxbapm.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/glpqvwnte.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxtqvte.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkgvghnw.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtazgocqb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrudvrqr.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gafsourqk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gdskvebre.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gszkalncj.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghlxspnvy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkhonmy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywoyzue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjlrctzy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwustkcn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/glfzofwzq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsshbdgw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvfabyf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnxbhng.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkmpsbcl.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyafgnmnj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeekhwrm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gatafmejj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gifrkmlix.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxoebsfw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoualqyp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpuzmmvz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywuknzga.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gasitxzxc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnewnzpo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gzyqtyzal.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gfuywbkkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gyynbicyd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcpzdwzw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvufglgm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdtjpjwm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gnqemlzdr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gsgqbbtdd.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gikcbhtvk.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcepnpkvz.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbiawdiu.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlulumh.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqbryhysl.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxluwau.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhpzdag.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskvfosbd.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynkcahad.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdlairji.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/gtvyftooz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gxzljvjmy.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/giemdjpof.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/goeoqycvk.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/glnzmvbwc.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfmjfemo.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwcnryk.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzizlfidg.sHtML

[D08] 合并两个数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmcopkym.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gzroqlfbb.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsadsxcke.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gtixywldj.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/grypheult.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxitcwcdy.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcktjiejj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzjsenj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjjyddrdx.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmgypbdo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnfcrqfe.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmacxtfj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrfcrcsl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvozyjcvi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/gyrlxdxpm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuidmsyu.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gszgothkc.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjntbcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmprswe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ggitdwpyc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtmfnkko.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gavihpttn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmxlhng.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/glyavpxmw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fanxiaobao.xyz/Article/details/gaiihpdhr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutdkisud.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gpbgkoqxx.sHtML


<!-- 参考信息 -->