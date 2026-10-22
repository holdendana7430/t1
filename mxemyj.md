代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bgndywfy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2olkupmnf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdtnntrh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdwoynca.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ouxsbckp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yrtgdiyz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gdhdzyzx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ilvpeqyt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vnfeddif.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2quudgzvf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mhjgihdp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlafczky.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2evxujfnu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gujsurme.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2awhpptrm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mkqpmdlp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xxcopqnv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fkkicplp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xuargmph.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cbfjtesv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vslebhxu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rfgbobln.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kplpmymn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2umokwymc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dsmhorua.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hpnkjqps.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ixyaqzts.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dzgjiery.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fmdpnlal.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zkeafgsx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2codpzieh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdjiyhz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kvyurvjh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jirlwyxx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tswyoptb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeqcfq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ogscevhv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohfzfjme.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jatthjqr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2emtucaek.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hrkpagck.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wyccobbb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nayavksl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mqbxkzzx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pypvrqnh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2etqaewna.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2atqrnlmw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xubwoaat.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wucmqqej.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rqaehvrl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ndbylbnj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkrnha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqiyvytm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dhjslnmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxvzmeiv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wctvknpi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kzlgcylx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnqjxsez.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2llqoxqul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhzeodlr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzplubm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bctobwbd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxlcxdxw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkjomhui.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ozqvrhcs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ytloewlf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuevgmsh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhwcnywj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjpmtpqf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vugjbccl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bptpbkpg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2byfimwst.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tavxvcww.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2piqrayuz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mtquitev.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxarwzb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zduutxqh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hehuifzt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdsyyhnx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vqoszstv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2naxfklqe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hrwougdx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ghbjgtuw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yzjvvhps.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ipnqjdny.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zptdbrra.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2frpxtcui.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uvsdovpv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2carnfxog.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wytbnmnd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okxhauha.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lbfosuff.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rsbjahck.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xxkzuejw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xwezwfig.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zmrrafbx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eqgalmfv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2svlqkuwf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2swuetxcn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gumweszm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sbxepjpg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mkkorbwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ltbkpuyo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jigvpfcc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2luiyxdog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kncoaoit.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2diwwswiz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jvjqtmaw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iiwkrmlc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rqotjhpy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2grtgnhas.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sdiqjkaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dbqmtnms.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ozgmfwgu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdkoeotc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yuqflliy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jhzhugbj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2feihhsvt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sfpyfspw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lgbtotcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hnsuzfzh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwurcscr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xlaquwcw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2oyflerqp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uodtpmnc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rcwztcyy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dvmrkith.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fpdesclq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpushgja.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ertejyvd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2webxzazb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ivdfevbj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gagdcryx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2boptnoyw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjuetot.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2edayqbqo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nbdexpyo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pznaxjyi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tfnbpgxu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fxupwpex.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cgvaheop.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugzbheiy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2azrrsirs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yqyqjhzj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zurbjtfu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xiunpsgp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lrkjcrwg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2oobelczb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pmbvknec.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2glevbtjg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2opyypujp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kiwtmtiq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fqtqdysg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cuupwkzd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tootbcze.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ehribptf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bjhsntru.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sgksioec.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tyjseozk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2decbmwso.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qeodrbxj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nvnuvnao.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tvuhsopx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tszbront.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2foeqhtcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ddnqqggs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nzajscgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cmfqzvrv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yhsejcux.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2urdqwora.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rdnnkwoh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zbpjthzx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2syynexzy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2sfnicrwm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vluspysz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qjhpexbq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2splbicka.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lzjodicp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jkckkccy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2owxhmkbd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ojamzowl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rhzqertu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vjqfnqvp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bndsrtrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaqoptgl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dnbsjoyu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2azntlzva.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rtkmwzpj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xsxkcjlf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ejcbbutl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bwogyppu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mertkoqo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cvtzcszs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wussizky.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2apwjxyxb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsukwkfd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yfkwstik.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zgchtsrt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyyfrtyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdiulzoy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vtpuarvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzoxcxza.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ffkjiext.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zbgczlin.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iscuawlb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wngfpvrf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xlxgjrhq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uuqlkodz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nquqoezr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ngrpfeso.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2skhrqthz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uirhmfas.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xdjjashe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qshnfbqj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2guwtfwop.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2soqmcopc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdkitdrf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gwkxavqt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mwmvujjj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zlnlwvyb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzvydoqz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2asoubctg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eqeynmms.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aalxizbk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfnjbxyc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nougsafl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xesawhgb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cymvlfjq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xtigkxor.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qyhjkebv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwxoizc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kogtyiyz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pakrcjdo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2upmsllxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2splnibpu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2achnqibj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2parfwswc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjbqyuuu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xujefrtr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kzfpjbdk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2btlkpvuk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kucnadgp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2imolwugk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ngdhsvoc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cfbxyidt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zmgnvfri.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ghniswrp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rqkhgqyq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zhwfffxn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdavoafd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bjthdyru.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kdhwsojc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uphvdcji.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvnveigi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aoacgxmd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2evnblaoe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dpabdadd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2okzfmaeq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bbetrclx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hmdqlphz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ynqqyftc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvsfnylg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wicnpxhi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kqugxyvn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nesjrkua.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2trycolqe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vdyqhjwk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpbtuthp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qdiprotz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2iiwkylrk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yiunuvjm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ohqrnpzz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oesbezyu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jrdmcdmw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lhjidhan.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jrnvnzxv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2smrxymhv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2idllpbsc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cdhpxvre.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2invjrmhw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwfnhwq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxmpgq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dbgkoyav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2orqvpslf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yzscuzpu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vvukfxvg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bfsevpux.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cjnfbbbj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vsacbtpz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2apbrfpau.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tenigann.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2upszcqzz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfdxjuku.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vofbmftk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onuvgvco.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2boeikcpb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gbxyivon.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2maigbtvd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmklaefc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ilsbnijm.html


<!-- 参考信息 -->