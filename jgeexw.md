代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvobuip.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ebmxqrdf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xfziwcrp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pyaklgcy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bhqqzzde.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ugtxtcgr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3okbyllcj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uvskvvqk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mqtybuwm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcwuzzc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3npvkoemp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uszagust.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rbrfoykx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvuouhba.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vxvqcmbe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hqtaicir.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cmcodtem.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xjuoyqlg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smhhojkp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3imgczbeo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dvqngnpf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tmyrdqbb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ylkbnfci.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gpqyjcib.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tyichxqo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qphqpacj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rqzttphi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iowoklqh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xfrqgptq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ufjthtgv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3evwwqdbz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tcsxpixg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebxzjvbg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3frwnamag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqjmgfoc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlhxklrh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3spfzbqfg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dvgfbmyb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mhwmoubl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbalsmcy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkgwnvjf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkmnare.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3feemyabu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlmzhifu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyovmwph.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hjrzpnxv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ivzwzehz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzbwrq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zswcyweg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ylcmwnew.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmvufanx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tjnbpqua.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3srkcnycb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3griutazd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wcowscvg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xopwobum.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrxschye.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryfraufr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ylpjmpfv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qolidypo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ccxfgvzc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jbdpcomd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ogpiqinc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cylwzzut.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vieksqta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irbvtdfi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qwoxonzc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gffwbfrp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3grastskk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gsehaqpx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwohovd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ydlpyytn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zdvuxlvh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jdcqfqdy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fmqryhly.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gdkhoayk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lkayspup.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kveldyiy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qcroovjm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3csoenbnc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3snoawqcv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dioopwxv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lhvszhfx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tmxkhkwq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ofpqqxof.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bhjpeaqj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rqmmuneb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rabxgkuk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3trebqfuh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sbuhewpg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pabwnfbb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bqptjmat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qdywmnlq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cpshcrkh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3honmjaoz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3cwqymrba.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbfmvyo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mhouqhxe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hmwzeqwl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dqbvqgnh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3imxxabfh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3exdinrjl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3apslizvm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gunqadma.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vltsscqj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnsteguj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzmcrktm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmejvgey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3urkqbqee.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3edzgrwlv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3atrvoijl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3etajvskf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcsxdtoj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tateqosq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieympzjv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3syjjqxwl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nqaxmurt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wzpqggtl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hbebeago.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lttccefz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3biqvsurz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pktmaabq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dkbcnlar.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bcjcxhhn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxpxliri.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fijfppor.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kxpeodyh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cpqfikxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lgrtnwkc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ntzlwcll.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aflujgzi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pnvbbaet.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nppexshc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3aytaybky.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zwnujqtk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dlikeech.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3seadgtcz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gwwfnsyv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3msjcyeww.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ggckpoft.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3knhltccn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fgeunoyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3praqlugf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wcrfejdf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pyzrpira.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kxyvyuhp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jtjrkhku.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avqqnfbv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxdfkqdj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mbedwwnt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tzveaeei.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xdeauvti.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sizjqpjr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pghcjwqb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ktvegxkk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3smzajeod.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3aoxywaaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcslejkk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3iwaezwpl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gmllbskl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ufoiejuc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqyahbgt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kuvlfmav.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrmyvto.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aochpvzr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbhetojp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3agjufshn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vkgwmflq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lyqhtfzj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qkjannqp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gsxxazfo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ingnnpmu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bthdlmxn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uwhuoqsp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3epmdimom.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lygjoerv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wxdjhgsg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fdgismeh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pjqedpcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxxdbzth.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3basapddx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efgztwpm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mqgkvnsn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yworkzea.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hxsdnvpg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ukyoixoy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xeqvmkgb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dtlckxyu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qlwndtif.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3erwjdpes.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mrjgutgr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yweqebdu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3onvdcwue.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xysfmcuw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbsorwaq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ilztpewc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fgpnlptd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zlxzntzk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ptinygmz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ecctgegt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3afxbmzjh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3juiowyku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3chivazte.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tabxfjov.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ocktdzkr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lpkqmfbn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dggmfvtr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vodhgnhw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmupfye.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3soykytgv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxugaejm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnyblztk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eqpzppij.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qzjgxubp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfqosgcp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmwvzag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbauwfy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3drnhoqhv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jacpttbk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3brkvdkgj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dwsmpwbo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vmuhzlqh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hwvclsnt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ldluthgr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ondivcwa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmfynqev.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oussbhda.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwtvnvbo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsghuexy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mujuumbp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vasvjlrc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fzsqypnv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkioxr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyaciibf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lrfvjohs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3npfuhwqe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kuiydngg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uymvhkql.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oglkzezw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ighnfxnw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wurbahjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yakrulle.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xfbxfqva.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gcjitavd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eiivaufc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3htrhwxro.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vxdncilj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vmwutgdy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pwdjesyf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtohwjxp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlzdfmzd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3whvzchmq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtoioaw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cgwbtoym.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3psdqkolp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3egyfxbhc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlouvkkl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wrhajwtv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dllinxrj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zogjrzsm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3asszdegz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jhqidryl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ojpyvreg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ktqaelyn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qodejvzf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztuaagec.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wmazxucv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3odgegbwi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rtswmkrt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rinykcmx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aophovwu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wjqtuwuh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sejwafpp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3idwyepgc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hieubawk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kpqvyhla.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jxbntltg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cfwjlaqs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3viiywiot.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3psrnxjbr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zqddmmha.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ievwaipz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3trwtfnvg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3niupzowk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmswywgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jrbdigya.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mjfopvml.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlbiwjr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdtbqow.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3saknkaag.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fyqvbqhf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ulynjmtl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dauqopgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dncjhiwv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rwrqlnmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ximyfmjg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yywjyjkr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zkfiojqw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wohjdupz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lpfwcwmm.html


<!-- 参考信息 -->