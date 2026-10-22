代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjduwbo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipyzucvs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ghszapzr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2itgxryva.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2idpkuvhh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fiistdtb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mlntnjto.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzyqbui.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lobktvym.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cfiuvtqc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pnfhbabx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2afjchxow.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ygfqhqtj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2iaygrmoc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2swzkbypg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2enyhqfun.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tmijebiq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iyjkohga.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hosrqnvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbgsoszw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eirfgkqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtfhxiq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vjnldbiu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2iucwzgfh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2drfdkiyq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwohhfpd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bbdddigv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gbnzjsjz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zgiopvsq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbbzboov.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jitukdcd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gmiclopz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vqekhktp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dkazcwby.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qtfdxozf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bweptbcz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqgwpvrb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xhdcurgm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lkcqiwkz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gsaofgyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzjpmtqa.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vvxvoemx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adoundyt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2otckwksh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2twaxsuyx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2odghruna.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhlaupnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xptpqphp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqkbrwxs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2sqaqackb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2azjpxrpo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nkhtshwp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcozihgu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cxmoljkd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ywxsihjr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbdyjfex.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziizosex.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ondqwbln.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vohvkxnf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zccgczqt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gbttrfsn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tpbfzcjl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yqewipln.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2favftxsm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvoopbnb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eymrixsf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gncmgrxb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mvmlqfbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vygkqzov.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rsubxcuc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxvqvxbw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtrghqsq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhmmdktg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djparubo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mjkobxwh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mhioebij.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xnepwrgp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mokdywgy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bkqvmpkb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2frupedww.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bqabmkpu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ebvyaajd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jqrqoeas.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hxececvb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2luxmryvu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oqcjetaa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jrpvvmkm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2urgsvjwq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kkmrejjv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ghtrzhkz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jqgsnrlc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tneeflri.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rkfardet.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yrmidfmf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rmarccrw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xcotdgtk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2idksunjy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xyqlpeam.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2udzocxtq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcnmbcdx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qswjqxra.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dqzirmvk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vsfwmdch.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tjezxigh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bycpihoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ghitlnwf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwgfbj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xuvttarz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mkacdmpy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zcvuthmr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lamyhbkp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zgociyay.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hszzacvz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2chyouhtf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gslxukbe.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zvbcflfl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqefeetr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxsnviob.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2myiqhtwl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2quiribet.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xbujzdnn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjvmiqjj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwgmeau.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wobloimt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2muowlgwr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2situumfb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gchbftrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kqjojbad.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yllymsig.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fldgsjyn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yczthwrc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rhuxkkef.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2huxbwaiu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mhfmwxfw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jclyswzs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kutfovqx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bjfmgkli.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jsbnzwky.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2irqvgpmh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xbawknmn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bgrlxarr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2sxqgnnjj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yypdyjmp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kaqqtnsj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iklxzjtb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jrhlkzqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hytyylrw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2foiifgdr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wdifyakf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nkbjtupy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2asczagia.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mqncbaka.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2goiscwog.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wweedbup.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qthtabuz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eiqnlqwc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zvdoqayz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dbyngwsx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2okyqynod.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yfwwcgdl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2sjbzevja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2irfyepbh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qantbkgo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2itgrausq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmvdxvu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrcqnnlh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjyazrl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2knlehtkj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gkmukjha.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yemxbfdd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jkgktszt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hxzxdkdc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnstfsdf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lgmaeyqr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mvjtngda.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fqdlketc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kxrnjqct.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fuhduwor.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zeseexug.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vjxylhzf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ekegisul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yhrpifjd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2apypotpi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qziitiur.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2iimzflph.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fxqrubcw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jcsidmfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrmcqvmw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jrrftlmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqdubcoy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wvnhjjxu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hobuzokj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rtzujooh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yzngpezz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dxckedyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qrhsuhss.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qnkcrfje.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qtloiuer.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hlkjjxtm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jsekullo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ovvfgbjo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dfyufjht.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zjbchmlv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlhnwyhr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gddksjjb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2iuyrcotu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2csokloxg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pidvduuw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2eduyfzkv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxuydvcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uozcmgnv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xwjzlwdx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nsujxklv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pawuzswi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2irwjqlwv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrithsem.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gmidgvsv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cnloigip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sastxpxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzhuzvbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zgprehiu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mangloqs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hgiizxoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2msguvviy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ttigvkhw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdforpfm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pcxvuiyg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fucytrhr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2phefugmu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2djteuuvg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cjjtkahq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lgsdveil.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xrtbuina.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fuidpcga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qdqtuptq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2exocgvwi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lioexmde.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zexkcfap.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vdjmcxzq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2btfmkfov.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wodxkgoy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxrrhnl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sjollfif.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2yasliigy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ugpxatcg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dsdpiyqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfjjkxns.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfyhzwip.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kjxawobw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ehakzufs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xilcwtdc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dvanvpbb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrpufxf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cdvppuzb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikctncmd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sorhyvyz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zdikatxz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bxotxanm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kxoteral.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vopsyqqg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vjguyoej.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pagxnsvr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ogsvjgee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cuvejecq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgneixvb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2enbxvfxz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cvfgshfx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fxlewfvz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtcibaza.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hjkgmlea.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hteqizbs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eqcqokau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fnctcftl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydkxtene.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2koeooqim.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2afpnqhwj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oqisawhw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bhktqoyx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ydoiysjh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2easzvqff.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kzhcxpgv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hudlegtf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhexmjmc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2izsokloe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pqygvrrl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qkubshvt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqthsosd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lidmwjqv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2egkngvcg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vxiirdra.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wocutlbu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xjkueszv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fuqfqdqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qyrvhxwz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tghuzagg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpihcad.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cnuvkwcz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gvndeeqh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dbtwkxcy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ffgitvix.html


<!-- 参考信息 -->