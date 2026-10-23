代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdusbpba.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dbroiaai.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ojaltmca.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rflcutrm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3eeblxdqz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pvibbcgr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngskyebi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dbfcguin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhrooagm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pnbizwtt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ottqplnn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfftrzc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ydrgxlll.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kfilmhcd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bmtfqghi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xtmqpyha.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyhflbra.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3azeswtvg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kivajqoz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uukdgqui.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thibcael.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfffkarp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tnnwvqyy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3brtszjjv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ksjmttyb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rhkhbfqk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sbvkibpw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jekaoebo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zsrmirna.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hwpvggmb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rjduronc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mbzedvnq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pmuhjaib.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zrsowwtd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ilmttiba.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vbnlfxjz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfevycz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jfclyivl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mkhtvfkh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kmtgwkje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqwqimtk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ujywitry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clntvxib.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yjpvvxkp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gpzcvqrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exaiksmd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dkbbhiet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xmctimnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ruvsxfyh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hsliefel.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kqqrrmjm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfisfubn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vufzyxxd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yesjhfhz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijnntqj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rvthexef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyeykdsr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qrchmohn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eeabokyr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3erynbbyb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pslqoqfo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hnonxcbb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3eccatrps.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pbyynwoq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bxcqaxrl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxuogbd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryyjcupj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjrcchy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzrgvbvu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3flnvvggl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfujjshu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qnfyoygq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mthbgmua.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ingagzcd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ylzhyxin.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lrvesvuv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oxhbhuma.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zhqzxirf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqaaznmc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hhwftzuz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3guysowpv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bbuhsnvg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ofusjzhq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yzsbpdjt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jmezrdwq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gfkfhlbk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3egcwbdxm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wldwoecy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wfbuktxq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qtnzpatc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmyscu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uhvjndpy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qpbyqbtd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jvtiwvsz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jqhuqsio.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pekbwxyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3alcizifg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ncbjhtfl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gfognmyw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3raocshed.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nopuocob.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3glpwvlxu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtmhschl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ahbglzgb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vuageleq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ievxmrtj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jnsehmxb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dhwhhuvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jakbqajx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mgpptqkc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyoxeary.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ubfncqam.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3varmcwvt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3inqnfsfh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3weqrsahf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bbzueglx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwrqsdw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3myrvrrsr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3apuvrtkx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3irltmsmi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aygqavit.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3duissmjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqvbskv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rjhysvzz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jcgxbqnb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmzkjt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vlzbcart.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hnnodnyg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gfcrzhtw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtqegu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lmsqpwop.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yjisixjf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oaxtbwfe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eaitibrw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3twmaksaj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mlulpvcz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yahcsobz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vfmwcdha.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ohbmpimg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ebvptani.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gyxitqef.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ubqolepa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kzcoqoxx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ytvjyslo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fhwmpxja.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3czdfopma.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oyqmpcyf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3eejudujo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rzwlxobj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jeknizwx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3eiqfpaog.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3brgobjqr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hvjxoitz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtadmmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3yjuorbwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbxbpuxy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xupohzft.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fdavbcnz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3eputbsso.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gxdzuvid.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kzpdjesy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mpjtiplf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nsfjhabx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kdmoyaan.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtpamwxu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3asrricce.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3alirtunl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nqvlbfxd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pkgokpdt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hytknaph.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3szintfsy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mzsrwlly.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oypvcobm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voxczbsp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gwjkntnn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rcdylbvp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cmmqrojz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3unjuovos.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tvcrteut.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tlkvoqzh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tvnfwzuy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dlxpbcpd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fwqdspdu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpqslpnx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3eutcswsm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fhbbkeib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ysvwyqpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxqltjfy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sptfzdtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lapymbox.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3subvvbyj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pfpihbjs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yvqinzob.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bdeizwgm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hsszeube.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ziomorts.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zjmkcflo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kfiyvpsa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jonszlns.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3apftyjax.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3whgwaiyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dnarrxlr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ecttgdmi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rjzddcyn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnynxqca.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yejxstjc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nzickgxz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oetodqbk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zibmkrrg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzkoaea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3trhvnmcu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3uxjneckc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ihtpnaoo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afvdprvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3poytanoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvjhmsk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3omctathk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ziuuxgak.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbkrfnm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjaruuqy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wcmvdoig.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3urtcyhow.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rxfeouce.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3efdnxpke.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3newruzii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3klldcwnc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xhpkauce.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ewizwtfh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhkfylef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3puoufsgq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jhumhmst.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pouftwfe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mdxrjepi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hfxicrtx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cotxohkj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yymgedrr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nczdlgeu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfruzoyd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3edmhwtgq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wnktifwz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fceqerba.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmpcavcy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3flvyjjew.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kmegmzxk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3eleeonaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jxojnhtj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pxgpovvu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ekmbtoab.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mvgbbmgd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3byltjqtq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zlyrwqpn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uyrhciny.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmszytra.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3noysqeyj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3panfbjrx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hpfacbqn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lcwdxqwu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ifpgmxpi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmqchreq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3swlwhmlf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwncrxbc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkcwppsc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ofpdktcz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dtqmlngi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmhsuzxa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3asvsekjw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gslifcwd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xnydyyxn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcuaqc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nxzhvhmk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nhwbhjey.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mzkfssqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3enuztmqq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxxqyxur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ipdoykih.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uichdoqx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nbcjydpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jtwnrusv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qcuussid.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kyvbnmfs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yzeokxjg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3szoeiejz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3faehalwr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jcpdbwst.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ijwphtkj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3piszbntr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqtzzjha.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yanxkksl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zjjwwtgx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lxixyhsl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rgdxlcyo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cflaxtoc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmlxrvtb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oozzvahy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ojbsnifp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eodnlyww.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhpydzcw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3shcbxumy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rzyngopu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3axnsdkru.html


<!-- 参考信息 -->