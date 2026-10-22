代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2shohsdbp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2azbozqeh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlxdhykq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zrgpeqoz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2epobinyp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2adnelspn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2muhtptwe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2omrqpjqk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2idzeflxu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mynyvrrm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2chmgcxts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjobixby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zsjmhefp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zgzhtyjx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dqiatbhh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcgzrxx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hrrjjckp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2yscnfark.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xhbunzzk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vzsmlazb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gbixevmc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ppcggesg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfddnsvf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bxyuydia.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inajgddi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qighxige.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sfvqccel.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vueqvoes.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zlgnmcfd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ctkvlubs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cycceffk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rohpfdlg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ykkhorcx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iyralucw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2imyuqyia.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ngiwioci.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bxswybhv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dscpaqvw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zjvbgdhj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fpklpbzp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jbuvlbag.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvknjsf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mzkqbdbd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kejafisg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udccxsng.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vgudyqac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrntaxog.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ylmqizmq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bfcjbrkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pwyoihvg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nteoqzrr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwzidaf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czwxjmwi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uotwgmkk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wxruyiyo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fugijxnt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fqjrvtyt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gzkfbyxy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuvuepkq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdyoimcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdknvhds.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vbaktxtw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rsnkdyfx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qtszltxl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fcrvkdme.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pbuxhzoh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2owtmcdec.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tneustid.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxkoufqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oadsiekv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ervyhzdn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2scggbdvi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ujbbjqlo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dgyljldg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2khvukazg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2eiuvspdw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zeweevwd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zwegredq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2etuescpl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wmqqmmdx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2yfdedtgd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ycgpzybx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dmnmyydn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ntyoxirb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dvaxvjgo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qepjjyxd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zgstrjvz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2axgqqppz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2clzntmji.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mmtjablw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2liuqdqjt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qgxajccu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ujkmziic.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hdbpxrzh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2pnqknthd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tgzityht.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cxlpixgv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvrteklf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lsfrmiyh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wjzrhvet.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oupxzzoi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lzibqmss.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jktpykju.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hnsimffe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfbfvyc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2sjvjcvzp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wetdrqxb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ljkjipca.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2uetmmvvn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fukkpsgd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oxapnzrw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2axnecvam.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2thiisofo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mhlhczal.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jvynvcvv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2yvepzkns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhtlvxtr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebsevezp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mntinxlx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uogkrzmp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fretvjfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dmnlzvrg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kfgqgukh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2heedgtqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvnvgplj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cclpxedu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2chcbtvzm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2geytqxkk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzhyuyft.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nnrebvxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cgauyexm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jysecwnf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2queslego.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdittzbg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ikpmlrrt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pgjpumck.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rrirxpkx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xqsigvjt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qjuemybz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fnggdwwm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2azarqihq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sryhzdvt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fzlslakh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qphogpjf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jhpqripn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2iauskluy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2piizhbif.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hxymomrp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yqtzperq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2emoouaja.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2inkbbhqw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ltqvcmra.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qfpoylrf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ftdycuzl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eosfxtqw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nlswenev.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ukezodeh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uewbxxnf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2evrwthvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2usjqghzp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wizkbapr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lwryxqis.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2faiqbzrt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfksmuf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nwqwgtsu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xjsvobme.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sllohgjv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2crqkrkiu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jgarllck.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vcfgvlga.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2laskfflv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ahphqmkg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zdahqkvb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxxdfocd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2uxzzpuxm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2atgwcobn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sbimnuig.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unjtcsxr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ndgjmsgb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bblrwiwj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wqjywadf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gdmrulte.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2sluwxzsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rvuodkns.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dhwdoyul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mrdsisur.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uxyuvfwd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kctcdunv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ljvnkqty.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwlslnjk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jcambpxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txjbxvvx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2eqhajkjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brinfqaw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sgpswria.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xmdjrqff.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ivkecafp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uymccqgw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rxutcufr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2htgquigm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rktafamr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ldjfybwi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ejptwkal.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rfkwpuqc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hjcvymaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2znwghbdp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwowxkad.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kpevbkmf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vluxktid.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdiwysvq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wvfzmwta.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgegezxn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrnrhkzq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ahotlsnd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rklzggaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wudhoefg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jnffduhq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sjmyiemt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ngashiwo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftujwihr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpfldcem.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ueawexwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bclrvgrm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rsovftmr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2acevdpae.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tcudbiuj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xiwtretc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2egknpnzc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypjmwvoa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lmzbtgqi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dptgzxtr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uaknciqk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wegtfzyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vyrgsjom.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2efeecoik.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2smyhlcxx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2krcmejxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qrsmsgqe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gnokncoa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ttuysfhi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nobcjerg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lycbqdwu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2awknrzcj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2quhkwupa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lpgqnsuz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzkqnirl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dnarovca.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wshawmdf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2okvugwgi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtpjly.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vpzlqpdf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2afietdcl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvojbl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzonxqc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ychopnhe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qztjfvfg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvbmkkbg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2aojjsorr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bfoalbxj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jtrifqgp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gtagtbyl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rxsnpbcv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hrxtchjv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2huyxtvlg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqsnwyf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utrjuxvs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2orcrmysf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xirfcqib.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oafsbcze.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kbpeaozh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2evubahuj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nklhdvtz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2altxotem.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nmiqhdzo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mikatkns.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qgwlmubq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqjnexd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fknbjkcx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2exlaktyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dvumrvsb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cyrtuxyo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cyyqqvoo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wqiktdrt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ikyhizih.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yqfttkjf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hegrsalj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dupbcdce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zlxxzfzn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hpsvhmmz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nnvwuwnc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hrhncjwt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wpjwnsli.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nptaizau.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qldbxafr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ggmfkhup.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omfqmiif.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkyeakf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dyrkuhek.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rcylouml.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcnihefh.html


<!-- 参考信息 -->