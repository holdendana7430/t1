代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kxzhvzqs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjdcgx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gtrgxyhp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zkcwkovg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2puwhhbzo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2chymxoaf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2msdadvba.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xibutxat.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tarpcojg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ssmchoei.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ljhhyebw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2raqdynfg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2soutsvjc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ohjvgrnd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjdghll.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2htspamtt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2twxxcqnt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qajsglix.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jhzgcruh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fbulgdzl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yponwxoc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tsazaisu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2likppjgo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2eukywrcw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiuxhsuh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpwkmnw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wuqapura.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pskxmwln.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwyigrgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nokgfddg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fkbnnopq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2uqdfggci.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yzkpvwfz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ksvroyiy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ivsdzkns.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ctevrkmc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vacrrhwr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpwhjyei.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nkhgwbip.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qvymnoas.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2crxcwrfv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bcdwtifj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bggaadtt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oykmopyt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cubixgnf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pvorxksf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gpstbuza.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fckrjtnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sztxlaly.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nvqfvobn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qttcihwu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kyhtwzov.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lrcnarxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlrlrvrh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggttvolz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfdjsmpu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zozzpuno.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgtslmfz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jkzeksmf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evtvbeym.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2laghjygp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfwzih.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxgcicc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmvdkdir.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zewapsow.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hxlvxaig.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2axyziylf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xsfvyueg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ggkenggr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddqlkdof.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qkvcaebr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vmnxixps.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jgvtpoym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbjmgmp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mkjtwkxa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hggknvjj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dvnwhtgj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hqfnaygt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2adzzmlzq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2uxrycfka.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oachlilw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ywgnidqg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jinpbnyp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lrtspanl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wcsygzmt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zwqsekna.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eovdnazj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2npgluvbv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nwbyzwvl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tpqhatfc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pfbwvjgo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lrwymvuq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wbedndlw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wsyytdbc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ueluwwrs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mktursmn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gwchybec.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kpbljdjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2afmcftmw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gwzywmte.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lgbfahxc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pquklbhx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rdbkvmgg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wveqbydg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2njevfsru.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pjrfsbaz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zdxywxmo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfsokwj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nldnyfng.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2sjealeqc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2isvzoold.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lvnfknlu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xmajyfpw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbnpqj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yasgrgex.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kgazrgcj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2etxgdtco.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxtonef.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2phfpsjur.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2igbkmbwb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ahwugetg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jsfndcay.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jskiuois.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bnviiaoj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rpyczyis.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wykwrwre.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2voegokzw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yeuvetnt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahuixyym.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fucfbezw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bvnutdmc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iqudkznw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2anvecyxt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ebcigxbm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pznqnkys.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zwkdjzbp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pwhrgtha.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dudzdxrn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xbuccecu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fclqltkx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdzxjgjp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bnzqkfhj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iwmyugcp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pirtehwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ziadwwbt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dnyudede.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ctawatoo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvcpbz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pufjzpyh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2psjvjvgm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ozwjjqbe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jmplqizg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hzsajimz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2glcksutl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2enwubvqs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2iwqvkkza.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cumjnfqo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2undevbpb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mcpneayb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xvllmabp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cclhecjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvwtmztx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2npwwfdap.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxqoej.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmynlntt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2azwrzosk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gujfczqy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qrtljqym.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xvurxlaq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2awyyjnbh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xnbcwosu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lhhhjtcq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsymmkvs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nyalodmo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2flamezxo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vtyadnlm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qbrzfget.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgbthaef.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vlukmktf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzbbhrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gaeckqnd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xocvtsby.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nxogfttq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2muwauusx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pyntnhgm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cvbsdwds.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mobowkev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cootlpix.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wlwxwyip.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2anzclizk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2etpqzwmc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkeefdpw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tbvcmpjn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfjheush.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knkcqdgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohlmmuth.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xaoqraxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqnqxzid.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uukovxtm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ywlcpdwg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qcvezzmg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2umldvjrm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mtohswzk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fmnrsdba.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rtdirpit.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rbsqhpbj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tmckwhdl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ierjdted.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ilspfwmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2edrningq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2piglkomf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkmroxxz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2minqwlvl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mekpneny.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcewjrl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dfgszdma.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpjxuapt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2boicmbxf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkmzwtop.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yblfuxhe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vccojlkz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ynorrfvq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvzotej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qokskacj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxmvnznj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hbjlniav.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qweoncnh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dtibayru.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oiaxrbxp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ftejepwj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hhvjcbfy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gnfzinyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wrqiemmu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2irtbghix.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2aptvzeqw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2srucjngs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wvfxfkqx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ghdiydjv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xjtolrkv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nlnthruj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ijvdmqqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fdrzoirz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dsxnoonv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gthhmybk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfeixcao.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utcngrgr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rbibhkso.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fkjribdq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bnfjsxqp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjritrii.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zixatpij.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jlrcgult.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hbotqgcp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wpocnffn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sdmqjwsa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzshnmqx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vrnbwefq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcenraxm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pivckenp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kmuozikw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2itujfwbj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kbtuitww.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xbrdlyhx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zcjvmxex.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mmxwdvvj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzhqay.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cvadfjav.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rajylqar.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrwpstq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ikxxbpyf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rsqghbjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uonpnozr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqphuius.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lommlhaa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rmkqdfha.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmbqhmg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aapxnymd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nxdbkitu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jxwzyedu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zdsyskag.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2scmqeeoe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hycrwiyi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqlusad.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2guesjrsx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vwhhlqxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hxipntib.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2liqwltdk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rmgwqxpn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2irllihss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qmbkmfua.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkghmyo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dviyzpzt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ytuuznzp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iaspfvpc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aunuwhek.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fehirwyw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bvzruvut.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2evwybewp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xstritzy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gnidynaa.html


<!-- 参考信息 -->