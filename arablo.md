代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgfwdok.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ptzdzwyd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cnhsmsne.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bhdnmemo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xktpvcyb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pkshoyww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2idkmvhla.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zenhhmlq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sbidfebe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2awkxckuw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lymsnqda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tvishuxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rrszbcgk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2elihblsf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wqcutsiy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2htjakvsn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xjxwpcog.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjrnfr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fvuamgzl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gkhrdyxc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdurunh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kjhhucki.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2szltumso.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbkfttv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lgqjjwpv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rtfurbym.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jyciylbb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwugktl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cbotufhl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zprfesvy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wzdcyuby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbzjizs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ochnczqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjrwqgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rtnpjsbz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qvkyqzmf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ojokfspm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjlacyun.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gvaxgfyj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chqmlwrz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2laiaeqtv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zaexkwrf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kodzacmk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bfoagvgy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xdhctxjf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlhinpq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ukesaasm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2plwtsadp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmiruijv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dnswvfls.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2naqppggk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vnjydzrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgfsvqml.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zcisqhtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yikdbobk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykyzbajr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ixpgigwc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hieuqkmx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wihoctfb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hssnpuzy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xamppimc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lpisohwh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzazicys.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abwsihjf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tghcpisu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xzihhujo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vtiwxbtd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lqkecepq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2slveclxe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2psscfokz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kslqytfw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xzguhezf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2svgoilmh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ivwmdavo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zfwocbgr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmmdmq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cwgrsocq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2knjibslm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkokieaw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nxslompl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2voggkqvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mtfjjtep.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ezzldtpu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tanodzzk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tpnaimst.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ibosvall.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bbadvpcc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xetgrdeu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ddhginlt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyrevpx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxndrjif.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wcmawmfn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2urbotunm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2etaigeaq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ubxalbzd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zyrsvzge.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mtzlfupe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2loygkvet.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gdprtmnz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wdqpzpzp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vfhugnhn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qppybsvm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nscalzdo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkizxkrz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bvewdsiv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tlewanzm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vczsyrsq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cjsdiqps.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ranroiol.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tvrkvnoi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2krxvirdj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ukuovfoy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fxussjae.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2eulbkwag.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tlssidlk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ngkcxdjf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wsyvlwbi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ueolvkuj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mmmuhmje.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2evwklfxw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajbxndf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwcazohm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijnfkwv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cxybpofl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcppggrk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2agewmtlq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ehqlvohd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rstmhvpu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrwtuxen.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykactbse.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ngyylgzg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hssdhzia.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2klgqyurw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rtboqxlv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzojthx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ejswsufk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iqzykzae.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jjvpbzsr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fobjnfxq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kruhsguo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dzrytcbj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aeantbtf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzdapp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2sftwthau.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dnutsjsq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2phrrlapm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dqhlsjch.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dvwrtayo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xutzdjic.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2glceirqy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jqsijscj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gddflujv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dscvuysn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pstjgdvn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lxeuyzkb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kmyqsvza.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ahcwqljm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wfrdfzzh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzxhyb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ywjksosn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xsrsiedq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zmxqdrho.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkrucdha.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ywptxnws.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vdhzzplk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rdotptcy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gagynjlp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cujplkza.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ydkyshtl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ufmtzqlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cuqxpgdh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dopvjmbw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hsaydjbx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2faaodgmw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2poxcywsx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ylzieech.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqdxttbs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hwlgdltu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zciwnaqi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2loqqunrr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qtonirdn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dpnbeean.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ewtetyuo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2admlprrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ponbzzxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zdqwwjqu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uerzbnfv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oeftgtxr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uysiiadf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qtyfpejw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2dlzlonzo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cyhyxqoo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vnwozecx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wmgohtqv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xcorwpzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mjqnxyzi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ezcpmcdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vnpvyyib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aysinjvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iisggqyf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xqhbszmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwwzxmjk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xzcrlprz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xgrmctle.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jyomsvkz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xndsftbe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jyhajicr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qhffhvir.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xxbbhhyw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hqkqjbsq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2toebefjc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wfexlqti.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mimptsts.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2eljzghkp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ytemiboh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uqjfxmbq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mcrrcitl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wxpclwtq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2npwmzbng.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yjiznffq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hrgudsue.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onsjamtr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bpkbumln.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ksauiugb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2djciaram.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pudfsgxv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ukmkzeti.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2oztvgsne.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2beiswtlw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnmfncug.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kalylzsw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2givplsmi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2oeeklcbs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nyafycvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cedvmkvt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdfhcqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxnsjzav.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvrriun.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fzkejipj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jncbsykd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ixpiuwfx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nvqvblcy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qubskwan.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2nwdrdrde.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zszgphag.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qbduqvvu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2urxtanqd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tcpjycvb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2trojclxf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkqjsxas.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvzpcigj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kfwckgzs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kzpwnhkp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vakwpvuv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2osemwdmz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wgvcivtr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rjaeflyk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rwaccrtc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnmeqvm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hinobxrk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2efrtmkfx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qliksgdf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2iyeaogdt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2voqbpqyk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xyxomvjl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sbttvcmt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpnjpjxa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vyplxkdj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmjpgg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2umhalwet.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kbpuscbq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fiqoxdkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mptvlegi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aeffjfji.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2giqgndtf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wzexubpc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nglryxoy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hfhvzgsv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vhcdnqji.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rvwcboig.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2awaqzugc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2twipjlit.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zdolsxrn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gumvvwko.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yaogxiuh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qgnyebxx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dokbvkek.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iwuyuxtf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qtxqgwbx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kkuuivxp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wczkiqtx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ceryckyh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ycfewurf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aoulodid.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ocmxfpwv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2codvwqja.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bjejmnhs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jkltsqiz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvnglko.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qnzpynyu.html


<!-- 参考信息 -->