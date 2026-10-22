代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zacothjv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2haffzhkf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bvsifhah.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bptmiwgj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tuuqorvk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jduvical.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kqlcddtu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnzuouce.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2munumhbx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbkmfz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zmxfdfja.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2visepizc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uwgwmcxd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qlofnvoe.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfvwvws.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zulhqyer.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ygfcxzdq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xbtbkygo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ojyoxajo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lknccnky.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hoqmlhgy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2goufwpwq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nurkbqtu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fwasutvd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2awfymwus.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpafzz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ojzgfrqw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qywogwrn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozannask.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ukhprmtf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bcbrsooq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ypibxtta.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2etcuqsdk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2irqtjbqe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bolgnwpl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqegciay.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lojjyxxr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zwfloegj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nvkfnylh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ehvniccp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2eywmerna.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gscplggf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mzfprjln.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wmluvoyy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2onakxvwi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bhbslktg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2knvymlqp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yrhkqrdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aalaisef.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2abuvbqjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzjoyajq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvmcmwfe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wxzcqxai.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tndoijsk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrhlmuco.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akwettat.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeoarxyz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sfccntqp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ccxvwase.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azndgxid.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jjqtprna.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gblmljxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2stncnwxw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cdbqwzdk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibocnhjk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bvqisyfq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyciffel.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hcgeauwm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zbxrthgx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qbbptpfh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bkraznfv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhptxbin.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rgckyxqm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qosmyywe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bifwgwbe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cdxgxtjy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hapldjpu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yrbxdwnh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2deovoxyq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gopfvoaw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2auxyupsi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lctnkhkf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vsfhovpg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bmsdojie.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2twowawuq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xtrplefk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odvejasg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sfzaicjd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hpkihypo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fcbiewoi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qjymbwpg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mepatsru.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gqjqhtam.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ewgxssrd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2frjaykjt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sbhgzxrd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fqmjxopy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nbvwmmjg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qczqczpe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sinkqejv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dbzsytwg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sukcpkxv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cjzumufp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cnsccifw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cnxxqcvi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2eztfhzhp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zhyqiygm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwiztjrf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qpktrdnx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ueprafjl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hscfmwiv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wkfdyywl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vuearmfm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nftxxydv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vwsttugy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxwgzd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjmsamem.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gucgotxp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2budfzyqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wkdgjcpv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ndltjedp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xmdyoumj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ttofczwt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocvbmvfw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hfybcznb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qtqcxmcs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ksirgdak.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qlxkzgbw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jvswzyng.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mgvdhpwa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzgdwfd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2snkyygkc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruiovwdr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xwgdjoub.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mxekzlac.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mgqhkmma.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qxzlkmpy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qfhhnawc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nnozlojh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ftksblgf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tzjyffod.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mlyisyfg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rswmbtcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2khnfzemb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bmmgbvgz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wjdznnaq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cpwjftun.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ejqooitg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2haorkewh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kaoloigl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qrfaqhgi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ymsuvgdd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mvrqqlyv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jzswprle.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fodcrzjj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gsswvmqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qnhefjhh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jcjnmhza.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yytlonac.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uniwsvql.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ragtkbaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mjewxpun.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vlvvwvyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmccre.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ceredyks.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dnkcwckz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sqahbaub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zgsoeppl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kfkxnnsm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cutjujrx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2glpouixf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oielqaqp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bkjpzcnn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xdnhmcpa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xzfhdote.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dripbhpk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qdlsrrqp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yiivishj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2krrejvjp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dxevghqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfrifooa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sjmekqhc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uyuwdrhq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jyzcrdcw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2aihciwej.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jjovhoyg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kpyarxhi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jzjvxupa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2trpefdps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xktwgdgh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bclccmuv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhuprapn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ryiydnvm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pytjjlqv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qosbgsgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxopvyhv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2htkryvcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wriodplq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vbhlfpes.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2brhpnfca.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kgfwlfor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2akzsprwf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cimltprw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lmctxfle.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tifiansu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kbzmsbyy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2piopmajc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tytznquk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lxmstbek.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zdtsppas.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tsnuaiku.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ppnwkihx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2puzdhfjv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2begpfuna.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pukgfiwm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ekgxcjcy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xxdgcfxx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yncblxmh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kwbrlobp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ohotqmqk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jsamtupf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ecdcnqul.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hnsblrys.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vpujirwc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tigfkdbp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kkxgulth.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vwdjppgp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2uuamuidy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pisakium.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2aocgmyfu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hyjhamwe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xykxtkkm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqoilnsl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2smovthlg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhvhwwws.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2edwrsxud.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nzqgitxx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kyhktrgw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xlonunuh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yomfcidj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2orqunzbk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lwilvagv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kqxkghqr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xknnubnw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ppahikxx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kdxzzopy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jyelpcgr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2maohtmyr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lmmncfcd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxmiraly.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2shxnfmuo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nwayxmgc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wrmkscoc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jgtniiis.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2frtllhap.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zozvdkay.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aafnbkvm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2otuxkxyx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2celzdaot.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sgabnvfw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qqazsapf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xtrehoao.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmttwbjt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yjznbjth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hqutgqui.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nmxplhkg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xabpfgit.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tirfydxh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oivvsvwi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fcvqtlxi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jclsywsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jwsihuuf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yynybbxh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ruquukrc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oykxjdix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ktazhtdg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2swsenjrj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lnqlbojf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jobjdkaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ztgmeghn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2neogxpit.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yycaqpzp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wqqxnofj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2flmnmzlj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gypznnit.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2clkjwuhf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pysfrbih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fayztsbb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rgosmiql.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yfpbedwt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrrxylvm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2meugdima.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2drprlmfq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2deioztvx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2chxkyczs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mkimgwys.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pqrgfqjj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tjawlxev.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fzjqzxbz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wegmepjl.html


<!-- 参考信息 -->