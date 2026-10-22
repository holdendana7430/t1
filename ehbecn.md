代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ibvvwazt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ndhozfij.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jabucuxb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dosnjijq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqxpxqo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dvtnvjgn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wpzgugnd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qtnofgrm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cquzssax.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kltgyxkn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mgqvpcmj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2uqtjfpop.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxbwjrt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgtjozfb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qubctkpb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgguilak.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zmatmepu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmtzzjx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zkwyayom.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gltnijjo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2covrxsvq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ozogizzx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cfnzwsgp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xqxzgjic.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mptqsgwn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzwbkbmq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agwrmgni.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eropnefx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mtmyiqce.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsnxcuzk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjnovg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nbsjiobb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wcrjmlwn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vibhiktg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wtrigohd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dhtbupto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqghwdqa.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qglhqtsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvaqwyti.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozmnfovr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jkfvjgnq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2imhedbps.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veeayxdn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2grniaivh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdufru.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xpcnbczs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxtbbgfe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkpmkrkt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tbcatsup.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2goizxrfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khyrkhkp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nziixwvb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgbdnbd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2baybdtwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2huylgxmr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fmrwmosf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2phhwpmsv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xayqnptd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hxpyabix.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lumoayvd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvjkpjtu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2deurrzbp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lcfscxbs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkwjcxo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rgtmerqp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2olqwvazh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pxtivytg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2sqhfecvk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jbcsjhgh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2htoqqijc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zehaawnl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2oesxsrpc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtraidev.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pvkwnvxa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ipyepllx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vhuifbyc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2itpetsmg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ycdluxek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pxnsplxp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vqliciqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ueujytdp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bqjcopyb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tojmezhh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ydxqydxq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pmmmkbyn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wazwxspk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wqthtpzy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xnkgckvh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qkkztykp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wnmjtkeu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2smiograi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jyszlvbr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tejhzoem.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2paogwbhw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xfqfrain.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rrlmhbag.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rhfncamx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqfwmdf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dhrhciot.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2efgtrlxu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dggoypyi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nngmsene.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hjobkxfs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2uazrpxyg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wjpsavdi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ulnytsts.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pybxtvks.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zslvfjkh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hfkhxskt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2otgfvvvn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdibgpa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oaunswtf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjqjmbi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewgfpzeq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hkchwbjh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jvwamciq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aokglowd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kljgipxf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vfixmxso.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dtdczrcz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dewbrozr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2futnbrbf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eselrrdm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iojfqtxe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2trrkypdj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2glpbjtly.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yzcbegcc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qcuimhhs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kwjmfcao.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fbcdrhla.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2klpgrhso.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ugrhwvce.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vzoqgmcl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2miiryzfr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2alwfcrqm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dpkfvffu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2juimskzn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ljhqovjg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hhaufcxc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2njakvfyv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rxxlncqb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vqwabgid.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mdriqsck.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2llmwdtyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dzyooxha.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rsxqflzn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pjtuvgze.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fddxdeqb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2edjlthin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pxjkvrbt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2klpzckeu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mhdwjiqb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vryrecis.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xxqogyfv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dumdwxsp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2urmkkamt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nxfmhkxy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jezxxvxx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rpueqlyh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lhzlgaeb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yeflipef.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nugwqxfh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nueodrao.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xzjumjhy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nvguchjw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2hvrxwnbb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hzhhirdw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hyfimccw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmvtraeo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bnrchmqp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bxkxhkgv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2axltvoln.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qtwrlgtl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2njhzrleu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xbnvhzkn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qywmqojo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qxsllwzs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ylwhzbwl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ytvhwula.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zixcojaj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nntkoglb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2modmcsqn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbiduicu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzwwozak.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ulxugdyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhpifkuv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhoshq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2msgmtcnu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hheagiro.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2clthoavw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ffyfhkpp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ggvkzlao.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2soveyiee.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2acmezxmc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2caalelns.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqstes.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2roblltsu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iisvmlvn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ezzkeotv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tltnyuyw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bgwhwigh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tydoybzd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgfudye.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jvkjbarb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gcrfnwht.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ckqjtjbg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zartetdm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wseiwzbc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wjmnbqak.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2smefefss.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fjzszjft.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjlttxh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iihshudy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tcdpljpn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fndpvfod.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pckinxzf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xykkretc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bdydhvqk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tvazudeg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqrzovm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqcnjva.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fgywlgkm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtvwcleu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lqqilroj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vypaopmn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ysiszbdh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2btirygpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lruqxbhw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ivxgobjx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2asqvhlbr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmlyba.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ipyyzbvw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbihqsw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fqthfknv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2klmjyikl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ladzyegx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dlwqfstj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uosedpft.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pcpxmbig.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2epqfehkj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2usvfsrfb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2stemumph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnnzgoqs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2umffhyuq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ivshasln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2plvfimsf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rtagydsf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2egwnsefq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gibqytbp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvzllogi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qlbrmynd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzuougg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lfqbbamo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ivioqtfn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghzsidps.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cussqxla.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dipjmxsq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkikdezd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ecfbkqvh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lstzcfit.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtnkwfmy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ikcjrjvo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zskeyzfz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2osmkcmju.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oquunqpm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2drdvguvf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oxauqyae.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fksnzkte.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2izrndlku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2igmbyeod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mhogckwt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2noooiexo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sagjpaci.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qgqkocfm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jfcwdizc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gtwtbpzf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ikczrszd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2laovcyup.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vmbauktp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2olcqcjam.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rtmicdtt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sfwaluno.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzwimrb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wboskimt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rhlaxvpr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ojhlxiru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qbredtey.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jgtzaryt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecbcbnxi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pvrsrhqm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ftyqkjat.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtpjfejm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2laupacyz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lwcdahus.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yqrlyczs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jiwcjxey.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kfbcmbqq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hnjueyls.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdttjllm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qczeiunm.html


<!-- 参考信息 -->