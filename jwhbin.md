代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2roltwyoy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ffhsonab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dnmwczys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wsmurgde.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qewdmcyz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iielyyqy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mhukfnrn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmwiti.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ogdzyrks.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozzntsip.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exumcwqk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mbpvnylg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2swrhmbrh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2doeajbqw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmbdrc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cugpqsap.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2sshomybg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyohbweo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2arybiqtj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cjhnsuam.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjlrdgnc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ggndxipv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pdeloxei.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2thfuwtpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfrxzcwt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2gcftonbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scwdjnzj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zliaxayy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qymumoaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xjasanqs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2chbtmojf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2anxwfrqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgxgqyat.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vwdsmelq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2obmleols.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vndjlvxy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfezwnlv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2inwaslek.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ckaynfpn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2duogejuy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmjukvr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2scpknctg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdphqocz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tibimyst.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zbbltbcs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xunwsapy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jljemhjm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrueiehj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jflmyxwt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vffayybr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wihnahla.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2totiqhxx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tofsuioz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jbwprwcl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yvxfivhd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkbxuls.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zrmrrcqx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdpscywi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gjlyirzy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2raiiaved.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2yzonpeow.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqqpmlw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wmwwkfgo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fzurqpww.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cuhvgccp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rpjbjvxe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rsdapfxu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2doijeeij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gilspcul.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uobmysyy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2sbaujult.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qrruwrto.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xteeetrk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jnscuqyk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jjyqjhya.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kkgmqlbu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2epnmvabm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lgbxaeqc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2blrfbvpg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kdyfgfbr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dgguvvun.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vudpzwbt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbyjyob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqspzba.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2crznihhi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2coqyohoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kisdgwit.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lmfxytzc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oxznktrn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ibjhlwzp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kjkvhufn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zkerhniv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fcaxwlgl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlgsqsk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2elhejyik.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qgkjpyyy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xjvyopqz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqjsgzcw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hnkbfuzh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qspdbhlq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnrrjmg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jugekbfy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pgqndrip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hwoakhhs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qxqhfuhv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkdaikl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qztxgduv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ovkngldv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2edqbunax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qevnzfhr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hmrmmlak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekgorvif.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vstyvadz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtmtruic.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ojfuarye.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hpugsypo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2llfoqltf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cubbnsjj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mtiescbh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wyzuowgf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2srdtchgi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2drstkihu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lgajtcwm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2iwogfofb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dtktygzb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ghjslghz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2frwzedxx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hiosbaik.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ytrmeszm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gnysktcw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ssshxrcp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hkehuwef.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ohvqsbyj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lprgagds.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ybcqxrdj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cspvgemb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2omrgsanx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sqcjtbzj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ezblozjl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hixevfeh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbctdfsc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bdzsndfc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ezahauwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gcuvgoew.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2atyfeosy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dmqepbfe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dvcljris.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2evgzxkrg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2viceunlc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlrijltg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gfgjxyrv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fqfinnns.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yfsoaohg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jipchxrx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mhfrhlvz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zhzdqhya.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oavyxhhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgrbjwkb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vtzoafqm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rfsmraja.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kauwgbmp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ppcgzdnb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2pjbqdamc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tuajkvlj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kagrjnhq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lfsbdizq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xgivhaie.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iihxjgzw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dvlqcntg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2sszrvhzw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2colfifis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkjtjllc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cjxqueds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whfbzjkz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ogmeeyee.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zkyuqmmq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kxewtdpt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jthjvmep.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qykjeqlc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yevkcizy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gpzqgaiu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ukhqzors.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ssaatxrl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2chxalibp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ypyfnrns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2edtdlyhj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbhcsetn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kfsukqye.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aqeyurov.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dbwwuzpy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jomjoguv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxgkxuju.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ptwbjckk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fofiblyh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dusjyqmd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dvvqydlm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ykshaeir.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2efyznkou.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gqkfixov.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2quiqtmcw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2goopkpdg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrpquqqk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zufyykjh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2swgnmlyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sjwxpvnh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eigujoqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bhvvktfu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ccebvzvc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dfaeazjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lhqtgbmo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cvxwhjvh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hwsdnekr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kuqqhztf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ahhrlpug.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ywyzknzx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zvpbzdev.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ttdldgoz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uttzxetb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2agvclxmt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fsfsyefc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcpqddpa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2temkuyyu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mzcqdlwi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zppacafr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fggoadtq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlbwaqsc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xfzynwpq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pdwoqnzf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tnkydreg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2viylpxrq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2waiqmkja.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cxqhffra.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jczyoamz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cpcjghkh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2apvrqdck.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uphvlmxm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fmsxfqrn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oainbqdo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2goblfycx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2syduadwo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2smiyxqtt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tzskawuq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ivxgxgyx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jwxcnvpu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2drhcliap.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzcmaczi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2noahauwk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rtsfatug.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gvtotffh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hxciegdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uafrnwbo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hltjrtvv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqzttevs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2codepvgn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fzdvtbfi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rxsbnhix.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2utxvicqd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cfygpehk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uhocayyl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vksgvytw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xmjpumqw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ciimfqfk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zeidhwcz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2udzmsnph.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iirsfpsm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wqfkkefn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfxfwwg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2juubvcdg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nzkjoywv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2brxjnkyz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsbtjccn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gtwlgxkm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ofdtntlq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zdzneryb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sfgiiqsf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2supzcekm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yesykghb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bkjkvylp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lieddcbu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mlabrcml.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cebpezdn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yzpnglxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2iyqpubbc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hxwurhdi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jqswtbyu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nnasclgz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uecfcjjg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jcliwohg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dprzsjgv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fftvumoa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mezppoet.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hsgkjuej.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cvnnaswp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skffpcwl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tllbczpv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jdgrbmcr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zuiysaxc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gzioigmd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zszkmvec.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugrjludg.html


<!-- 参考信息 -->