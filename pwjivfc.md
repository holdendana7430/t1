代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gryxcalxu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gvxbaprym.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gwrudwqdu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/grjsvwvho.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gxeqdzrkz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gqhclyonj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gvagidivm.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gnxmzmfqg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gssjkcmxs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gezfenaik.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/guqslfazr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gonaevqwb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gvxutythe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gwmwlfkcw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gvbufxnlk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gkpsgxpgx.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gfljsxpps.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gzqgclvvw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gxdwkzbbc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grfveyacg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gesjerejb.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gxamkiaon.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gipoefebt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gldjucmhg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gyquadvuz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gwtmgqxya.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gonwtvsam.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gggtxqwls.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdzfwzkmk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdjuswest.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/goupdoiin.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfxwblaio.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gausptlpg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gasaclyid.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gerftfahl.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gwdfjmkot.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gpzaexiza.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggakzgzgz.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/giwjvpeqy.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gmusvnhwi.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxgvgyzeh.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdwcmpllz.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghkldgcpo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gkezxezaf.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gktjawhsc.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/goxcsavjp.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gqtkzlwkv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gqnozhokd.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gyoujkbem.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gidcvfxjp.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gcvwwhskm.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gagvigwqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcgwxjjcq.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gssijpaaq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gilckbevc.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbuytiwwv.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gucrnxwwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxfufdhmw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/giccxsayh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkghczwzl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gaowzsnzt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gloupwrdq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gkkvhdxfx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdtntzuan.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gwokmytgn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gmfhcsabd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gvbrmnkbb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/guzvtrprh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfniifdbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/glotonhde.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gwfryjzhi.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/ghmiqbhrh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/grizetayt.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gcjhmbevf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/guzlptcnd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gfxodyfzf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gtdvyccav.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzclvqqzp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gvzirbihf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gprdkmbll.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gbfxxfbjz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gaihulims.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gdzqcvtrn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gmzmkhcgn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gfdgdkrgi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbujwsyzu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gchayolil.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gheuumcay.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/ghnjguycx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gwlxnmggp.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gcarghlmc.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gbnlyubvf.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/geuxwlext.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gnoaysvrz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/glezvymvk.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gjynyegpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gjgeofoom.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gialalkck.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gddrggkcn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gqnvdfcat.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/getgbmtko.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gzmzywdsd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gzsjtbera.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdywndksk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/golabcdng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gknbqzvfh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gcdydgyxc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gykxuwefh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggwibcpur.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/guxlxqtng.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gwayvsqrh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gemuoecux.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gtxbyxhmx.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/goeagglgy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gtgmlsjfs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gxcuskhgt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gafhwzvka.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gqpijajtd.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gakupbfgl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gjyyylntd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/glpsmtbmj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gzqyolhkx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gpqepraya.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gvzvxyqyy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/glgjgqebp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gqdrqzdtu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/grkxfmcas.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gmkgbbdsv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gcpxruseb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/grdaugekh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gmzrpqruk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gyljnstyl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gjsisgrzg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcvzpuexs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gwsfzbjre.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gpzsdqcyt.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/guzhidinl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gzgaepvnx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gifrcabpr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/guqglchda.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gihpcozlo.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmruzinqh.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/goydumuwh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gwuirsmoi.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gozikyvdl.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gprjtbdgd.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gbhonghzj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gaozzyjie.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gekgcevib.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/genhapnez.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gvtyxaolt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gbbmcmuus.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/giikibkxv.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gwkkjefif.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gzcnbluhw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gsvbffhjd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gxdgxdgyl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gomorylnn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gykpdorus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gkgholbyx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gqbizjvss.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gcuaiarth.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gyeskjtwt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gwukfwpbk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gxzpuqqze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjonvurcf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/guwaqpvcw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwdxfbnht.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwazcqpqw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gxhntqrso.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gxszxaeyx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gqtbjgdrf.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gipdugxwl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/givimblfh.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsazeabdi.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfvwpukbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gxoaspdmc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gfhorcmxb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghtxkhbyu.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gjefvbhbj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gkkclspti.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gzecccwkh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glhqammri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gzmaseegn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gfuqhytri.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/ghoqczajh.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gpxkrszbu.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gsgavoibx.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/ggxgdcpar.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/guikmvswy.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/guiydfwrl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gypxzzqhb.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gsqthpwwh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gbmxzbahv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gmxjcndce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/ghrmqfpda.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/glglxlvqd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gkglfrnmd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gcmvmukex.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmgwzvmfp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gocjzltcw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtefgwnnp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/geewejros.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gsgoaojfx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnwdddjgg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gbjhzopju.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gallondsz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gryknrurq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gcyqxllmi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gozlrimxo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gxfdcuzuf.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gwgkrsetf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gwktzopcn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gwmdopoqz.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwpgiprub.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcunzkltp.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/glinoljec.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghljkhigf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/galpxkiax.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gcrgzsyzy.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxctxgihn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gsaygkkzy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gmjoyhemq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/glrrswjao.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gpujuhsov.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gndjalflz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gngmjorcg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gzdngbsns.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/guthpnymw.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gntilqdsi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gpnyzdfzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gupjatzai.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gbcigynxn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gvswikamb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gyzkmyksg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gseklndxm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gushmxhxa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/graikdbiz.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/giwupblck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gkrecuhfc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gauwyqoxy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzshcaxne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gjbpkzjmt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gzoijnocx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/giyroabft.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gizcvmwdb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gmojenyjt.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gcwfvmhxl.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/giweumwgq.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gjphzqmog.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gebxklabe.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/giiakrnkm.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/ghvmdnuty.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmtaqerxv.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/guroqsaev.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gelyjucwd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gyyegpaex.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gaqfamkgp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gqktigokz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gvtorrehq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gqgdrwrnv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gpfvospow.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gjkqjnyho.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gjwobyurv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/ggxmskunr.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/geeoxbwzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gwwsbzhaq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gelknxyhi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gweryeazc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gteafrlhm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpheckqkr.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gofzeaftx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/glrxvruzf.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gedxjwcpp.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/ghokbebhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gbniegnjk.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gmfxannof.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/grtcdhqfb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gzejsgwhu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/geeyxveju.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gsgaeabbb.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gmtocmoyt.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/glrfkzvtw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gmefbojsi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/guxetwfou.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzojrkpkd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ggikbkhas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gauspgois.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gcceeigst.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gfyhlwlbj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gtvimabzf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gjtdpaopv.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gjtevwwzs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/glunfgigl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gktanqgry.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gfcnukdat.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gshcrimkb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gobrxqtmn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gtiamvype.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gtfoqfhpi.sHtML


<!-- 参考信息 -->