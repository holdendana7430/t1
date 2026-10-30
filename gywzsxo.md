代发 wailian999

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/grxtuoeiw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gavvgrnfe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/ggmvkdlmh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gjrigbykx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gqhjivrae.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gbyanivdw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gaxweipoz.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gebyxprtg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gyoejgwwo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/giwrgmaol.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gwfiqpyqd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gfpxekqyv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmupaebrf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gulbppjbe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gdhaktonx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gjzfaprhb.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gtihyqesq.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/ggvxknluz.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/ggkzvijjv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gvfphrnvt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gbznrvnok.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gzfteedzy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gcrmsigan.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/ghsoqomcy.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/govintkkm.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gbwronzzj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gwdxhvipd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gokvjubgc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkukjswig.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfmhcthkr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gelomcoej.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gzglcjrwv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/goyqqtgji.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggwmpnxnz.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gpvrhpnzs.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gqddkazpa.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gwjzjsthd.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gnzykoclv.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gsgtmstai.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvanckqak.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnuhbslkg.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkjwnndxl.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gookkckgr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gvddfvijt.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gnebbxswy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrtwzulm.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gekxdisee.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gxboqnqqi.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gjavucfrc.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gzgiixfyt.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gyqwwnxyw.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gdlvzkiyq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtwgfpovj.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/grotwprjv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygvxkzjk.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwvrkxgjc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gdlmbkmyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gonigxzen.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvvuziuhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwwsjnbqt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glouejqyv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gnuwpwnwe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/ggyhxfrlh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtqxdqldb.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gmzfyyzmr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gthywqoyt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gxtpaekha.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gystooqfq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvbjwapo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gnttmegma.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gacagmnpm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gustthzwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/goiwvmsmk.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gvinlezac.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/grlevdyca.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/ghupgsbnz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcvjrckql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gjvptibnp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/guxrfbnud.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gfcvuixzc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gjqteccaf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/glctommex.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/ghhnaiqpm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gungybocz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gflztzief.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/grgzwgphd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ggtidyjbd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/glcbwtojs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gzrimjhip.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gqxhirhfd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfflshcjt.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gfwjuaier.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gdertzmtd.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gqbeskwed.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/guqoifeze.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxbtvunpe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gadgmjyxl.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gnehokquk.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gxiaahobo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gptwaxuer.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtiywfeks.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gscdmlezs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gvjjyxoqg.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/ghfvmcyuo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/grrylnsps.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbjyxphfk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gponvbbze.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gwwypatqd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gvejhechk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gyagjllnl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/goqztdxgr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gappnubnt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gdunonrrv.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gndeeauhm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/guwjjtiux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gorerzfyt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gjsrwqimi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gaspzcvay.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gkwvrzayl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gctclezth.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/goofqludp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/glhmcfqdy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gunnjaklc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gdweoqjgn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/ghsjbhnfk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gnymhjrlo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwrsehabi.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gtnspohdi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/giwypaykc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gbjoncwyj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gvrtkvtcq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gmvgmatml.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gqawsbhpx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gqaiipzlt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gbjgiwovq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gpdiepqsd.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghamzcoca.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gkatmswnd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/ghzwybhty.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gylhuoddv.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gemyijttc.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gvfrkalho.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/grulvphbx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gtascyooq.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gktgmstkq.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/goajvuiyy.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/grdizboka.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gvguqxhkl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/glsqmqmmg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gqpjetjbe.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gzatvgkdz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gvswtbdob.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gzbgwbqli.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gbbhoxgtg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gererdcjx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqzaafg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/goziqopwm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/givuhgkxy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gdqjsrnol.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gzkupetwx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gcprwftnd.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gclmphaoo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gtwjkichx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gegklqpmk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gqiqjannf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqsfnaojd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/giaqsanzo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gstndnrry.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/godibdcfw.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gqagvnosz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gxootlzdn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gktyypbrr.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/ghjwlzsuc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gcavzjoia.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gqkpomjyh.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gjgooiexa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gpwtichpn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gwgypmpyz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/ghmcuymud.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gqaapssti.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gbxspskpc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gxkwvynrt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gpngwdeva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/ghswtspno.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ghvwhebou.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goguggfxl.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gxjtwlqek.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gbxjlitws.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/glxzsptkb.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gpoxxwymq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gyrwdewxu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/givfhleor.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gqdzohtps.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gqyqeyfdt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/griuxelqt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmyirwjgp.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gwuuujfzo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gtsyvvzzp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gtwoyjzzk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwacvfysu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gsydrqmsr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyvztjcap.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/geqgguqrz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gslyjyapp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gtfrkmyzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxivyxwlg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/geqinrjpr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gurcmcqln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gbzrbxarz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/glnxdxnbl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/ggzfoepnj.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/ggjfvqedn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gnqtlfdlo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/grppirdzq.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ggarifeqb.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxmvkehtl.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gkrzvkrjz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqekkrxiu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gytbkqewk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsipkkiwz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gkclzsynq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/geehmavik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/glmarseje.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gxekcixsg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gwnbgslpf.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gonewlnsp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gulwvchyk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/ggpmzvwzp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/guuqwllmt.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gmmhpiflx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gnuxjltzi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gvndxqtqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/ggskfiuwk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ghnrkgkba.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gyzvmgyqj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gzqjwvmnl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/geidqkaxy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gqfemncqa.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/ggnloxwkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gciefimgw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gerozirfb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gtbnvzeif.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gvrfauapd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gzdzauerz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfwhcihli.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfhzfgriz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gghtgxkuf.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gjzpzoxdu.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gzjnbdsdd.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gylmceosd.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gpvsfvcue.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ggyiahtds.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gefuzrzzu.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjkuvfoug.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/glebypimz.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/guoxuwnaz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gggqcgvts.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gtynhpsee.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkigyvbht.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghgttljqt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gaodzinyr.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gkccpoizb.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gnmdmsnjs.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gjsqrhjqk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gtrvsyuqz.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gjqdwdiim.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gzgiwbuyp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/glqdztprb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwaohhmaq.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gdxsqwhwk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gmhwxcqag.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ghxdtenrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gmeuharpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gxgcmlicp.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gbbfefmcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/genewjabg.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gjubbtkrs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gxziocvij.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gelvlognr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gnipwhhoa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/glyclqggh.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gjyjfojwm.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ggadjxuwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/guaciilrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gjtxnrhot.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gvkxlpfgg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ghfvoxwjf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gtadnozuj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gaaasgmbl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gwktczsos.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gxitcgwgm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gxkkbvgqt.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gnunbqbvc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gundwmifb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gfpfipiis.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/ggyujmjof.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gtcnqtdch.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gyuotymic.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqdrqvlsl.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gakfxccjq.sHtML


<!-- 参考信息 -->