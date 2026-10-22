代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lafwflrr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hgdyckxh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgetivm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mmagixgq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rpnkjndn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2okpwzrtm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oskkkofz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pbmfywue.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmvbtsag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wwnlikdc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ursxrxnv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2sasxfoec.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zdaqubge.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2frtgcrmj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsrpuad.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psgjnebu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hhxzzmvs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2onadcxrq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fpmunray.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nlczymia.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gbpfneex.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2arcqxckn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cwwpfioe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iryrwqsz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tbbfsrxt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bkfeyepo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pcprequy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wkgblmil.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lcobuqng.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iahlnabv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ecabsjlu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ukcvktjx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bjliramf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yrawbmmq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rbfouwtq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iwrfmnbj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jewpieen.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idlffqtx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xuymglio.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gddyvoql.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2amxxctuk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2skqlzrng.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mvpybrdb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qawpzyym.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhkdtmbq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ppgcrcdh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dcyzmjen.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ikrhdtnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwumzzoq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wjuqgqlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obcxkvkj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rggubzrc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mndpyjof.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaopgvif.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wsyvztyk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jdbalvjf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eqqotlon.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rugnzvbh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqgrjgtu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fzzjbcen.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2clkqzdgg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2urjqgbxb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umwllrkt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uablmkzf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnngczda.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qcospzfq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zyvqvwyz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fngowktj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ypatrlum.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2obyaakjo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gkwojvbr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2iutffkgj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfnjmuo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wihdayxo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqtodur.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrhpfpw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rccjthkm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ezbyqohz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nuxhsopy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rzsxsmsy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhxuwyaz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mzoikplh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xjdxibqf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zvewqcdn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2clnsvajx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tqoixvou.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ucyjzylw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jrxzxoci.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bahvfbug.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gmyeuaak.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lybfivyd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gbpqoxlu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ofuwbpyh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fozuvzpd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cdhavuut.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jhxbhexn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hvrynayb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2njjqdqij.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qvtcyobm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hhxwkcit.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrmwvbef.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jclpxyyn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hkkhwnqn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2czrdwnpw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jkemvuaj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2glooonqu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2oclrswiw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfvctvtp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sgeinxjp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dijuawod.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2frkfsysx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bqxutzrl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2veiqmzeg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ywdcmbpw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qgljojvg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2usswkpbt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixzhaxsc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lpxfezhl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsmalyhz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hgcuvxsa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2citdqbsa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vucpmibe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2frmmjkxs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfmmfpht.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2blqswjik.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sxaonmzc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pnfunild.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yhnwgbwo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vziksfld.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2srkmejyj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ukflqxnm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2scdmkupl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ipeqegwo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cuwlhkjs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qflcvmmy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugmctxng.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xhmqjmqa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pcllqahi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jaqzyzbm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gruklpjh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kvtuvcai.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ryqvacqf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cifxbdpm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wpuyxwer.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jelbquyb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2duhuiwsx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gqpfqecz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dgurtcuj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yjjnmwxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2igvcluez.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2unswgxvo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nspmwkzs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zxxbzjsu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gaqqxlgk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xjwnwgrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dtwxlbdu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jmgkoqkl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uijyxsph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qklsexqa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cbulotob.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2povbyxpi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqqxydzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eaxlzean.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nufegwlj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhaknk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dlolctco.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gxdgvjcj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mthoyhwy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xyfvvwtf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2keowismq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pqkvuxif.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ciumfnqe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mkjthpro.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pyvfakgz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tbogdglc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2piglopkg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pwxfytbr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dxidfbdb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gztgossi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mumrndka.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zejapqpq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcbkwptg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ttmpsfkv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mteoonow.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2svuyycfh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ifrbzsmq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lwlqaczq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zagmjwcf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fwerqmhn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qthsczsd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yjmmyqcm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czeccwcs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ulyunpfi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ozbyqlsb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyaigdlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmmzpsfj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kdhqgshx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foldbqzq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kcndebtj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aeclkurb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yvknrjkb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uswotgdx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xhtwwten.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jntzecil.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vhsxpnpq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ommsfmpq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dabvwulr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gooctlkb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2msbklfhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kyrvhlsf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsgnsdlb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2trogaobq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ypqdlwwt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2utvgzorp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfdkefb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bvtueusn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2guisrxku.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mebxzuzo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2irokfdkw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ajppogkc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2spyrrrat.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jwskczjn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xyumxuur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2myrlgixn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qvsutfio.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrduvcrk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qzcfvzia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ennhczxs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uxjigctn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzpedlrc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2efztrdvz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sjjrnpdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yemioodt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bprjdqra.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dxcgomjz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qxyjbubd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hbzkhgli.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dpfuppzr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zfkxvsrc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ddyvvyma.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lclvkzrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qhrzfpyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lgoygrim.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zzbspmcn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkfdibzr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovbowygb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgmbffje.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqzqkkrm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bpregtwi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qnygtfab.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rydfhrmk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hzfjmxaw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2upfglqjv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2suavyaja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xgqmldzo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjariwho.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2esahjcjg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rgxrtrio.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nuosqjcy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wlpxtyje.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmmoduru.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xervsbmd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2epvgqelg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fxbadzpe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2npviqznm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wuippbry.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jyiojhkr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjpvmzpr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdalfeaj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2whwmvqsb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hcpjwuok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qicsfpth.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hizaxlbr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ogzzubix.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xxhskxnl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2afnolgjt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fawkzfgk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gzslgjpp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kkmwkfca.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wzcstvwo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tknaaibc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2skhfwhwf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2htcfqgsm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2chxrzosw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nsgrlhhv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rsunnpnm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qqrzzfdx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nerkxzjg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ruvzmrvz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgeiwhw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srgdggky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2iwjizkwm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cwmqcjzv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uotwwkmy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alqdpacj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ghvyfikh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2riyrxllq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iytswerk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jldfhmdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hokypeqy.html


<!-- 参考信息 -->