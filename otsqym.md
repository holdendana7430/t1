代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2brfrfztn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wdfhjvxl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdzusou.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hjbrhnea.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aheqmunx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cgabxlcw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nfxfqpvq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rjgwndfx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zoivfdll.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtvjaeta.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kcxfrrru.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xmxxxkkj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2abjmhxnx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yqvgenlq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2dzlejfsy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmeayew.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lapyaqbz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fvfmqtco.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qxifaajj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pcxkpryg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zdwnssbv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jaenmcch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vhgjkgni.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vqiagkgy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fpcifvry.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmcnexxi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wlhehoaz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjececxl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wxgdgyyu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qifrrgsa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zyvlgask.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tfwrxcsy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vrhyrhpg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tziwiszc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mvpfvkfx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yrefwfjx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oflnzkik.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2acnxrqeh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hrxzegxz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mxzkbqmr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ykyjldzz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnafjvox.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jnxlktkg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xkiosepy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qiwlmqdk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cvukhwju.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ckxjpxdx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qptwmnhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkpobkhy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cwnrskoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eombgygi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvczaosl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cyyhjqtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bcxuqsbx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sirgmobs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwpgjlrq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtahsntb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ruujlavt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jwvauqgk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2arlzutij.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypcsbjaq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rbigjett.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ieycfkpb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jvgpeyog.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izgwpomt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wugknujl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2spcyyiih.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rliqdqcj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2duvxfhfl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lgzqdycf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jgtbolff.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kukskwxm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmcnzsou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrqtutx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fjymqlrv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2auivgaka.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tqtkanaf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cpudpqja.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ryjdxqrn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbdlgkgg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2frscqqhe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhrxxuqr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2suveepez.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2crsrxitr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tzgzckvf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpgegumq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utlvrfly.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ypxxouqh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mljbeors.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sezhizxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rxfxlglx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yqwsccpr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2turnwgyp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gxrcgkem.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tvhaqcwt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ghwwjdmk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hzakbocf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kncgllzn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2flgfjoos.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ffcuaego.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ngrvikbh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rifovcwn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vssmvcgf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2eyybnobc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qeuuygec.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jzinmcem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2smzljscm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jdjhtpph.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zuqivuxd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2brqrxtxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttbogplh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bzeddyug.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eilfpljk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cxwuhzdi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rqwjvrop.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2idsejiie.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ccglxvat.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kfqbyodg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfvwyli.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ehqzwjxy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmhxxddy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnokayct.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwuole.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2azofhzkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2izmugaun.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2krhvhyez.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2riqwrbih.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ykwklxpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hijxzqge.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lecmtvnv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2djrbbrgp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwfveyl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bgawylqj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vmrsfuzb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nfmglrff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2swszosge.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jllqwxsz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2crkjwzjg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjjtuvbi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ujbkdvki.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dtzyjfqv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2oyjcpwuh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dmhpledr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2owxzctpg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2noxjnfkp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2egugdzhd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jzipsoej.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmgfze.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bwxkdern.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2trwqslgv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mjjzkbuc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2sriztqix.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rgthmdql.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2amhnifmh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xgpyzqhv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xspmogyx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gexxvjsl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dwjovfvs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eztddlto.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qmfmynlq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vowzqneb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvrixyc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rkfucjrr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtmolap.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xigtbekv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ssnczbtj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ijsvzzrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ztymetlu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nzjvydvq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lghraeok.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rklhlqcq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aptoaaeo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmskeqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pdrkdxsd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2eqicsicu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ydjtvsgu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hivvgfuk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2flzvuqlk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dcafmrgq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qugsuesf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2klsoepzn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sqyofpqp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fwgrxaah.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2isurlawn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2srviievw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dnvvhjff.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ndehvyhk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2utpysaym.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2khdkqizw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2thzjmngx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xbldzoqr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glatsdrz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ncpzepan.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywgyqjfe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cjucetzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wivejmkx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qmdtotwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cserchql.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mvshrbwj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yaxgplih.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lokbygsy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zedlkkrd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fpbnmbjy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hwofyedz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uefazsag.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ttbncjaz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wbhevhvd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bfsnxmny.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uazranel.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sojdqogi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjhbnno.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lvbyxgku.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aozhondw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cwpaxaxc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xtrvosao.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tvjhpaza.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qidsnonh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pewrewte.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ptfalbvp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sbyzbatb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ydcgbywi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcyzfmdm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fuajdmrn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxllxsx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2altkagac.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mlgpwtxf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2txumarww.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlfreqdo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hhzronjl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hejakwtr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aegqskcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qycfzvzi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ayregmqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2oxkxqfsg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vguvguak.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cvqdrrqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zjusndtp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dqgidnlx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zydpslsk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qledrpqq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oojppvrd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dxoesxlf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vjqsepey.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ewokxfmo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjorphlo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prisuqld.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2syhhhsdx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qurpjcgm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xjasxuqh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2muelxydo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vshfrsda.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2itygkpog.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2octyhqyb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2nciatpja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dcuraarm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2stkqnumm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezrvmbsx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nqcuoxij.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2laietxlw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eakqrolu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sujnhafe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2efmfcmmz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxxcddi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ojbatutc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jozmwrkz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2udishnks.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fdhmjkmz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cjurijmi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdmuweoo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vuywnpqs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dxnmvdkx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qrcbjcdn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lrrmhzck.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hsaingjp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2awdjbfug.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cfbxxoqy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fakhujdq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2thumeezt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2afknkrcu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tgcuitza.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2adwytelj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cmboqstm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgnqorv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ibcmvmaf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gufxbibx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ehofeiab.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dglysbyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xndvtreo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2agghanft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fixphqwg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtbcjcbo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nuwsirmt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iuspvgof.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jilrdggt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxjbikyi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gswhzesl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bebxxumb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jihuozsw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ldsodioz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxbgfcwi.html


<!-- 参考信息 -->