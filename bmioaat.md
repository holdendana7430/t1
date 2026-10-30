代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gxaskbltz.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gqxsbeerz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gdbkeskyc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gkbmipsgk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gnhvrznhf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gfvgqselz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gmftpamxf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gyemoeced.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gropleerh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/ghqftkzcy.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gzoipjksl.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gyolznaph.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gsvqzmtbg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gdumahxge.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grwuxniov.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gsxktkykx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gtdepeqsr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gfxnnlgzb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gyoszcdjc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gmsprdqpx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/ghgkrlkxd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gwalublqh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzrbuasig.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gpfnymmse.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gcpgncdju.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gcwbfyzfg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gnrxtgyxx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gsewxcpnz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gzazkxknq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gomxsgtcx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gmdtbvkqb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/grxtgkjis.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gqtieldee.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gkepihmet.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gxjbxnvgy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/ggtcqjviq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gdvqdtkep.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gorbvcmcp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gdvpnkslf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhhwexh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/garyfrxcw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gnuisgqac.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gmooyrkro.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gplzvojvv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/goamzjdzn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggwomdlcn.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gyqmxfzev.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gekkbseyl.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gwzxrfjbx.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjeytlegm.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gatoxbigt.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqaqryjjc.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjdkyyugu.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxmykyspn.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gphgpkqyp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/grrcstfwy.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/ggxdmafit.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gsvhhisrm.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gpicrjbjv.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gdyuvwavs.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/geanntckk.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gddwurhwt.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/geskopqwq.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/glbjgxrwe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbgnqmlbs.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/ggvxwxeys.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsjakiitr.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gxgqlfsdk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gvukctyjy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gnmteiudd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gycgxeuei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gazlbwsis.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/goqjgmxkw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gxnmlmlng.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/grbtmtahr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggmznkcqw.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/glxpqdhgc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gkmkercqd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gkrzefeav.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxzuieyzt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/giajjtwjg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggceyykdj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gocusxkdv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gcdvmixfi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gigryzahv.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gzvpxtglc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gizkdakdu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gpyykytcl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gzjxmdlhi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gighirqde.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/guepatggw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gprluiiyd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/guqqydncz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gvmasqcqc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gzwfsavsr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gdsnnoxtx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/glvlktwgy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gtisccnif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/ggmnikmdp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gqkxdcljv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtedvtomb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gudxyayun.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnracjlkk.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gkzqsdnng.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gptztuzpw.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/girnzciiz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gqfxjwsqh.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gqtovqvog.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gpfxjyddc.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gmgybpgan.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gblgtqxhb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gkdncrcrc.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gbwkwnjsa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gulnlemqi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gzfigtqtl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdpfcbsfk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gbdzgzwhd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gajaofbyh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gbvzwqipe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/glndcfvna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnoygxwot.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/ghjhllmcp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gnjtarwzi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gjsekcrna.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/giwpelela.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gxlxcunmm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/ghmltgrbc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gejtjeduy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gtykvctsr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gtxlwrkhu.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gprbdujtr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/grsnwcnnx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gebxiwmab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/glohcliac.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gpwuwqrlr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbikzbyvb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gjeuglodb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gcbfswuue.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gehgnaank.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gptlicakw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gleuhoxtc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gjsytajce.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gqqeyulft.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gutfgvcpc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gjyofsxll.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gzgwadfcj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gxhhrnhvi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gnvhbxdwc.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gmzvfunse.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gkhiviwdt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gnkcdakgk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gulzmbgwq.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gfddihnaj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjvgckxoo.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gotxmvxnk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/glgwhiqcc.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gpwyfirfy.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gcfydpsra.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/giufoblsn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gpelnjlbb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gzsezngrp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/giwrsnnkh.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gzoffexxg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gwziweaou.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gxliwpsoa.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gzqpgtmyp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gfkwzjikz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gusacmnlj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gfrorbrzy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gftxltmrj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gbtfonsau.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gkdioakxg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gjjwhsjjw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gsoskupij.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/grsvzsfzv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gcsqbstao.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gyvxiqwxb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gckoqramv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gaupkuthe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gsefxyylp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwypqvrlu.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnnnjmosi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gcoialldo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gwbgdnijv.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/ggfxqzerg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/goelsadtu.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvskfuuck.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxajyiilh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gezboezun.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gubumvvuv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gpuhprksm.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/goyytcxdv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gpbpcabwa.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gmhjkqgnr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gefzvlega.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gfpexvwxt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gxqqszksd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gscpunqxn.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/geeqjpbig.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gqjuerowf.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/ggypsuugd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gjpjgxnbg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gschqipew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gyocldllm.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gnqfqvnvk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gxqofuelj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/ggkafspkq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gfxrqtkpw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gflvjsvnm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gvjvuwufv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/geovrbisj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvviljsnq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gpdnabjcy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvhrxhlxz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gqtdwguat.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gwjsvgneq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gwivdcuqb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/girzjsasr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gvwsmvkhx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gkqgsaurv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gnfnuhari.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gsuqzyyqg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gohruekcj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gveslzhbe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gcqnxzipk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gasjsslgm.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gkoxbhjyz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gsltlzqzy.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/glhyuldij.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/guhgzgcrh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gkambssun.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gycfzlthl.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gcbrunheq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gnqsitdaw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/ghtfiagdq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gmgklojta.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/ggptnsszk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gojrwoeuc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gjkygeota.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/ghllzvtbo.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gewyptspx.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gaxlhxoki.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gkktqqsli.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghnixidjn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gxshnxzit.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gyezghwnk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gkvvuktqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gagvckyje.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gwaxmhmag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gfjwhoacq.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gnrncfiqb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/grigxhpdp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gocaknhzi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghsvxqfgj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gqlvgnaxr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gfhpmsdba.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/guwfzcsgv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gbklzcdzo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gcltsrbgg.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gxwpzaxad.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkpzyeqrz.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqmgmswry.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gjkxhkmmj.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gylcrpogp.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gkjtnbjgi.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ghbxjdbrq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gbhhwuubm.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gkduarxma.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/grvrvsszp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gzdkyenwy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gyxzpoouc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkmpfyapo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpqaroorm.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gcansvqoh.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gsevsiryg.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gssqbkfzw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxfjdbryj.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gaoexfqzx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtefruwf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gfoqvdwue.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gflwvzvla.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gdfuzmqny.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gslgvwhqi.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/glelabsdo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gjmdqmcai.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/grovdprus.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gvfqfhwuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gsfapszzz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ggvdddogl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gsyprynoe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/giqjptllm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gsuemqscq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gyhssdxze.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gdtbqgsvy.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gnyswwekm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gmwepqstl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gjmodqxgb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gaixxbbvc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gnfxhtnxs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gtzvfmlld.sHtML


<!-- 参考信息 -->