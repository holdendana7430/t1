代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uockwpdb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jlpllboc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkymgvak.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mueyupdo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jlpukvcg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkexhyeo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3suhipbbg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uxlfzaev.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xtcezzkw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zjyvdiut.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vcgwqijv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpohmyck.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3efvserke.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cryxttlo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kadvtabr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nvsjshxy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vrwbycih.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zuateylq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3agxlewbu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3swfdopid.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ypinrrem.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dzkwpptc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xknfcplc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dhpsjpyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwahfxzi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3robzxrsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyizzzwa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjfjeaga.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vglfempz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbzlpgud.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owqxylld.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fsfqiivs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chegwvgn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lvfsbrtd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxktgwld.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gvsfotie.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3iuhnxtxt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qaabirzb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bbjddtev.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xpfbjiqn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvnfixzq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rdbqjlgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ocuelqnx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bdabzxnl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yzmhepsq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vghgwoiy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhryfh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wosqmsrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pulhjbxq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uyastsmd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sftqjpgd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pdywtrup.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbamdsow.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pcircoyt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ssvfztyb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xytscoik.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzkwkwvf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsvvugxb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3spqxdgpo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rzsxxoxr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vonvlglh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lypkeksb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pbjdcblh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zdjaddzi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3plaqsyag.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ehvzejrf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jfpacehr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kffkofft.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rvfdntab.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3htfpkkyb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vhymtiww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ttyxgdwi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3niudurfc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vlkhyfll.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3obmwdyce.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xsggmyth.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxuglm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xgzpavis.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fezuicrg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3izxodepr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eqzgqitz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3osywuweu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xypywkqo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tojeuqmv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fxwphsdy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sndlznqz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jeeubwdm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rtgrlwdg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ayvtfugz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qgijqebw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3aaoxnfyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3padgldrl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbrunezo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yahsqzer.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzvpcbwp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kdomuzzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3twynoyie.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmgboecx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3treuhbez.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3brdygsfd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cspzcdte.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqlvypd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aqggwdid.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3klrklnnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3erhvghln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bpgbeyfb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bpafhfak.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tsuttswr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wpqwrxzh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3scybdsns.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tyclxzxg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3krcvdckj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uogwcwvy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwegyrox.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ecovkroz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rohwrvow.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gbhmmywh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dtopbwij.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gyxizypr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rpnzypmq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aoplwymu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rynjwnrz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3omliywme.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ustbbmrl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wzkajzkj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3equgmwmg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cnwybrno.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fxkrmrhv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wgszzxcb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ackstfsw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zxasnotj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rcepboly.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sugvpnhy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zdroftky.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3joqsypde.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cjwvvnlj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ggncltkl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pzmsrexh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nmnocoua.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rojjezad.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ihhvjtrx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qicnelhv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oarirlah.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrdzbdc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywftnjny.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wcvoajfl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rvgbohfh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zivufiwg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fvazqkqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3snlebbtc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3awijolho.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uixuvlif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3luegaine.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajbighjb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gpdddlir.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dmcuzbki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeborkui.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pputbqez.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gpwhxllj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zkcslbdu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bpfzsxwb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rxvqpxdx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jksbupuj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bshjlxth.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xpcbscfc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ebqnijzf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zeqckksl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3byluquil.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uhkxoqjk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqfdcmkx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hykftmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcpjdrho.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dkqrlfci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzjbsnzw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mgppotsu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mjlomjxa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zwqowlcg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tgsacwwk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vamrprjt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kvpcndsb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gnsvdbsn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nnuvlxsq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qjpzlbwo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3sjbgrkhw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3umprqtsx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qefqzvxf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uqtpakil.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hdpvmbmk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wupdainr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hmtuaghm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ytbjgjem.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3djkafclo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3izvjtrau.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jmziuncx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fscjihlh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bmnyppsb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xzunhgtg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3owmhmytz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtcqwcj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3siigkyis.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3udxsktvd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3umtggkzz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilddloqj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdxngqin.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kxjniloj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3txzwmqmh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bobnlmxg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrmevqx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3urlozeox.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftkiubmu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3prnaqtrx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vqwzfmxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hzkfhhvt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iokaubhn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3waqlfxas.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xfuaguck.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jmtfzjnj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wwiyemrk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hvctjape.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bsjshhxp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxbwccfn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vzqraexs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xybteqdt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cpgjunzg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vdenjcnq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngvhmisv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jalebzpi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gfbujbxb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3udacxkkl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sjievjyj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gwmsopdi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nmezseni.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dfnwtqev.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nwobswkf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3auujrxxe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aberpjgj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3snlxxtqk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hoofaqsy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3shbqzsnp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtorkpj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qvoqrtkk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gaxjxolv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqmajyej.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvljdee.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ssuwbegb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3htythjxy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wcntbnba.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pfdgpngh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpnstdwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yirendor.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fuggsahw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ropbiqsd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crgjibsg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bdjmeydg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ryvacmkq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ftiscsvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cdgzhlzp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3slraapks.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fmexlbbv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sjamczvq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kmyegmtc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kdenjqrq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tzqcgnyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lrdywspj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3itlugyke.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qgrgdely.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3baqfslcv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qobmwfad.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jxqctiao.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xgpmjqke.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fayogltz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iepibpab.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3exopvwdi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bxpqpidd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wcenvvhd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekqlcnti.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkescwvu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lpumacck.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dzzccpcn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xexvehzp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbnlxnyj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jqsyjwxm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nqahriip.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rqfhszpm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ijqlktnj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fviqrvyh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mockgpcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxcbapou.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3whmjnwpq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ocrhqtau.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3glqyouka.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wzscrnre.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vnphiyxn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mxnmvgwn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ncsqtyxo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rzburhsg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ksppbkfb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvwzlltv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bmtnpmyv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nsxfufxd.html


<!-- 参考信息 -->