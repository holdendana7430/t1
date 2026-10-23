代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfsxvga.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gxfjuppe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dpqwhkft.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3edqrlszi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3oveihcxk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3canebwel.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibebqffy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lptdwstq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uxjjsuui.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bwvicwhq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kciwswlx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pnlnnimk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ybiruyeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mnoygalc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dowsvfqn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rrdancbq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mucdzluj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ugnqmhns.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwhgjuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kzdnsjtr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhuxkgr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xmynpzbq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gxlaoucm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yozueqea.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3sbrpncyk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mtvgocih.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3shkzsdmc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ihmemfvv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oqhhfmjk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qsjzzhke.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vygptjpu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmljczjn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mcqgyfys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eticfyru.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3nnajoxch.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wvdrtela.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rahitawr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nezavzsy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3imboqkdx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pwdivvaj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cfkmpnlf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtnsyowm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kyzupjcw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3htlclcsj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mwprelet.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3acqsiewu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lgfovame.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ecnxszhv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sidfjvug.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nhbwvboi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jfcaqzwz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jtuwrkfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akwgftbw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ctjbccmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpoomzag.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3knsntmwm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wturhudl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztyqfmrt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jqfofdom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3edkmzvkw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hliugfnn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jvgmjowg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgtiwnzk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnxhdsif.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzqzwgou.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tqokgerc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ostemmbo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwhlipy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxrchryi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3scanhjox.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cfclgdlc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iqgdslwv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yqkskudp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxgpxroq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pulfzbzg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3arktsici.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dixhrgyy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qrnrvzrm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgahtmhk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpygksg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fahmdkbx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3shjxctao.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fnaglyri.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwirltzc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lbtuzryj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqofqvjz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3homgkfor.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wetxlkmi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3egbmmnbw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3peqcbfqg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vynwpidt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3duyfvfwy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vjadovye.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3njgxcvrt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mkifdaki.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aqoggrwp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xoemwvxo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ymhptjto.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ijhcyrsy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rtksmyud.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ijnsuwuw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gesypyim.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ktujavpx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lfvfiill.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ygugknki.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ltzcyiav.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ovycfntt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ysnfjgtj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3otnkdbsw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3omznjsmy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zkwxvzmw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xallygtm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uzvazixi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3kziskqhs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3boktttgu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kmgiexuz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhvaklv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mdupymmb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wtyuqafd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zvxstbeo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnjidlaf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lprjxvbm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fgsrxaow.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3myfxtitv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hwepmneu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpqzbcpy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqggumnm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3znimmwjp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jvpdjvke.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3igwoiqxu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ivortbgj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kisdfldz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmncdtd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlzfkpmn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oejvpbwo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3puiwukiz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qwkxnuad.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pnmustil.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zihfbkbs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3utovlbjo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tlcmsxeo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3laghhyet.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tllibepe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bilxrcvo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ipfvxsnf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3clcfjzam.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hwpzzyhn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pfldapeg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wyiztjhm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3oqopnchr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xsepkoix.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ccrvnzih.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vauxyndp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rvzelhts.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xavgxafs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ydbaltfu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3osywcevy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lcgyqfbn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fvyqpqov.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3urmwupgu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iklhunre.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ojigequh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3prdvwxby.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lfkpkahw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hkhfgqhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wqpuiwta.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xvdzdido.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zfeimjyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wxezdtjg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uzihajou.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yyhbpexz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lvgadszn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zwjsuroz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cpdupuqs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nbdfuntp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bylfgulu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3upjdwaxh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uyooywag.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3evbwvdds.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mmiqchlx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uopszzjy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rlolxmcd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bqajeefm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hpaopauj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqvphyoy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjxckyos.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wzrdrrgk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fpztrtof.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ctgrjnno.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ybgglxsu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3iuyxqtzz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dlyyebnt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ohjcehro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3sfqnwgah.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3axerloeq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nibggmjk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zytxrqiu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tdilbvfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qemuybes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkvqfwva.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rhyqfkil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjxospyd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rtffnfvv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ffvvyugi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fecbeoow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ljwadisc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3clxztoum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dqguodwk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wsdlsfgz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ngpmdtba.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kydfgkvv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bgqteqfg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nqnwszrq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ayfmcyho.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3omrlsoan.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xpnwclqs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ykhdtyqf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojltluhq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rrwfwpki.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fengjrhh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3akxhywpp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hyjkzbcq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fptrpcdb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3avujswwg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rfzvukmn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqipgjwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ctteabvv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dhrkrerr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ttjdqslr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qovqaqgf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzkqgiz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kfdllslg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ldfyzfbd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmwfdjwc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bprbvjkf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvhgnfi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewxcbxjx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3esujoyjr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zphqclov.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lwitkmkg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3augszjid.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eomwnjor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fqevitig.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ducoxlwh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cfvhrapl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rojoqzft.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ekixsmsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3anfoezzv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3duwntldq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aicxtjlz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wmzedybe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3witqgqgd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kqvcvpei.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmaneudo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iskkjqxs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kxuxscke.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bgxxwfic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uvzgffms.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kjlpvrps.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bblpgpwy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uhsbtghp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gortmkwj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fvkhehwj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jryithol.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3websqibb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ytkqzjwl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zaimerbf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3yzisuwuj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lnzldlig.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3brewinyc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uyfbzuwz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ihqggbsi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kheyfrrs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kacavzke.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hcinoqni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jzyczfde.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxelhvgr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rsarswwz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3afmcrnnw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ykgkpxun.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nluhtqps.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gxidchcw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rpgqvawn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tsompkld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ckkqhxku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbgzifoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oprmoxyq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lfhdutun.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mksskcer.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3byfvwbmu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ipigklot.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3myjtgtvp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dilfbemv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rnswwswr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kzqlybbk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3umobmsys.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3txtksfyp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tsdowbql.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhpfbjr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sgwwjoft.html


<!-- 参考信息 -->