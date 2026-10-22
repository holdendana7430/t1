代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yusoocgx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2socjwlsb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hqensnav.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2imlkwaiv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2exvirhck.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2phishsgx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2etzjxovp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jazpgkof.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ekdetfjv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hywuymfb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jyuwtpnt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2skefkhxh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tovnehst.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fxehhzjq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2egwmtggj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vuxqeaon.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kneylroi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yykhkcag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gdivyflv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lvyrxsds.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hoelzcwq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xevqijmq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ikexmmne.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kuxdjphf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ulkjkyjy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wkadumdf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhstltfs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2atjkzaia.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptygghqy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sycrqohu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2indnsmcb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ttrakonf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ukerzdtk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xbrkpalg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lljjytsl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ecntuefm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ucqjffix.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2weypoelo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gdsjexpk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bqamtgbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uewsmuwd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kyojbtyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awpryfqy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsudsgeo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ylzuxsjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbxfdrfr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqcenyxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iygnjpat.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2icvrvfjn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bdcaixji.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dtsoelri.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqdtyvrp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2imzgbvcf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ghcfgywq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lulassdf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvufjfol.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2galwwjob.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jfmkdgnr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pudwvirg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mhhrbhtr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uzqwxufb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdnxwyhg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wjuhoilz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2myqszhpc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzvlvdb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ohquzcdy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uozobuay.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ctmdjyuv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ceetyhwx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lrpkrdiu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yiyunzxe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcusqvy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2guehmdyl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbgpsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gfgxivfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ikjkzifr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxubnwzu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mffjqejp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnrozmo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rpkwmtlm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oudjlrij.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tedbftcp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2evgfzasn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kljxbthw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hqwmhfuj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yagvpkgj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dmeppebn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2trzenemv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wduzevqs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2cpcegeaz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qjfilucn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ovnrvbqf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rrtaogkw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xnhlcifo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2msdwlwee.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kyeppagc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aomudcdt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2caztqzak.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2boegijah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmldzarm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sbskkvhc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xirzctsy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbbbbcmx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mbdyfurh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2buofgfqa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wqhaalom.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jyewvqik.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wywusrpt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2npguqfxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oixbyhzf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tjnhhtpp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lkexrnza.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2njvlewof.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbnzblmj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gejvqfdq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hcrjfytw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipeixlwy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pjypyvkn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xcmwlhrf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jvjskmjm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbxvlpy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2crfgdegm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzflylww.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2quzartcx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bhirbqqc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qtaanmjm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jchhswet.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pljgicjd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2egfufuuh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfwizuud.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2afqsbcto.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ruchxlqv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vfwamsrg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yuocjaqg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hprkwumz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2duzfqiqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fxisqhbs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nwvvgdlo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2udhflfvc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hzennnpa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zzaguqia.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yduuukpk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cvhohknd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tgsabkee.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2goficxqi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xfxegixd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pmwgqthb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dimzxrlj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cuwfbgrs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lcqjektf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tstdyefu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lhyfnhdt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qmxenwdj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twrmchza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eibqcrxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2neposbkr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqvebtra.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fanxgiwb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gjylgcze.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nhtcewlm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2svttisyq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vmsmzcav.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yjmshyac.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hytqlezt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwyqcwos.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsyjtcvr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xnikifkd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2diqslbqa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2evnbeyvy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2piudzcqg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nmmlbeel.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cyixteag.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xizffnei.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sgatyyec.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kqzziieu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fkyybztd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yapihrjh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jnjveidh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2spjplcme.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wcmfslfn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvmbot.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2epbtjauy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zjaezlry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2phuutuwk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2uoizmewo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qfzfalhh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2djobfnko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkfrbbed.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kmrvtlqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfghehqe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cyeewxwf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ojrlcfal.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bvwpqzyu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hsegdzdx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zrfmfedk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ullimoqa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xvosycqa.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jeryflxz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dddmmdmg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2acupwksx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nymeazxy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2twxnjbox.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2suxyidgx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pfdxazax.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pkifmbld.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqvfexo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tscnoivb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wneaepnw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2deoseiju.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzwvzbo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2saptjnws.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yhqycpdy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2itpltqyp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2arbmkaif.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnycwkf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zbcqcdvp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2thfujkkv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qtyvfzsg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmkkeclm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtbbol.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qgvjllkg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mjljtzcj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xudzlmgs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2toptftqn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vrtnggkf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqraxyuz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kphgqzbt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2blxdssui.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dovtddfi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kdslsmba.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wzfggkip.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xloaoigo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2klbcssay.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kidizaju.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2omfogzhj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ntiyinkn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unsdorwr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rfpmhetz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kziqlzxp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mcopxcuz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vyukwaog.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ctypbrwj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wfllatof.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wfvllpxd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tbpoibbr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yrsfitzt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gdkpmmau.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nioouglg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahztlhrr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tlqsqwoy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2brrsxmhe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qitbxdyi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmxlqpix.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2objbkxli.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2upbyelep.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxntivi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2myzreutl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xtiojpia.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jflxakyw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tcizkuop.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2txfjizpf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2akfeirfl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2axihvhwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eitfksdh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2einzadia.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2erynyesq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2doklvcaz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2akwxadcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqxxdsxs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxuxgkhy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eylneqil.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2byuyvlub.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdtpfzjh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgbjzvbb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zchmopyx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfbooaz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2smezlwpw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ubnodhft.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jrjzijub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pmptfhcx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zoewuxqa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fhtsomih.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qngxyqct.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hriotwqc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lmqswpva.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxkfujy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fetbmaxp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xekrlhvm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2semtibik.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pjkmplcs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wsgxnklb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jeeqgphh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pzrpiimw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qahrouaf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xvjqzgjs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftrcfpht.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xyedowmd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wcsduuix.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jofaoaql.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjssktjy.html


<!-- 参考信息 -->