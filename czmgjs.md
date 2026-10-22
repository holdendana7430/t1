代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wmycwzdy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ljvwelol.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hvgvymjt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jrxqsvug.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffmddkfk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jezkpkdw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2udqupqvx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qdfcwcrd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ddvlqcho.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuswhyjo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rdvijxtb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uzpeqewj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2czmsirbv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwellxo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrzdzq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmrlzgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jahhnxto.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tddmsonm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obbgxlhs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmggrmmv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sxocghks.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvskrddw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2daohywlj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psywjexj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxouobf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nimudetw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qmkibknv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgjjdbdk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpvlwybe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2iwxdcpqd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pctkhsau.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sptposix.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2puqocxhm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hpsidbaq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2weflyiff.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bvtuwmxs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zumvsfcj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ibvpopxm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlrnndu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxagfarc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ongklobi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rukyhnrn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kkhbbfbm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2raybjeso.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gsjrpwdn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vadqijnc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eqomzvoc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrffywnk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2korcekyo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejzqzqnl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nixmllht.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gwxkbrxy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xurzzzrd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eypbfeeg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mxfelptq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dppjgmfz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2widgupwb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hgbkuqll.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uzimiggl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pfbrgixo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hacjqkga.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2amjtqncx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vynsadcz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2haxwdilj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tfnsqfuv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2euvtrfqx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cuzgbolj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fpibvywe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pemmdmfx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jguvddab.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ygngncgo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fgihoqhz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gmysxafe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2niuceipu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmxgaxl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2slsrlnfv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkwpjxp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lhtefceh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvhlxxcu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ujnaxwhi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sskflwki.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ewnwvado.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2juwunooz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rhpcpxiu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtdnnkf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxlqqnmw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqhqwyn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2titdsspv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tjiksplh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdarcwjk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wddiiuvf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vdiejuwv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2spsrmlek.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bacugnnh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xgovtkol.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2owxteeij.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xfbdumfg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ibvirfbj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dknteifc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2afksmcae.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2quxhkipx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mezzecly.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zqtehtim.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ykiggsyf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dgmxhjgk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oscsverm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ncrhllge.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ngijgzut.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wrilmqof.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zruiqmfd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2skhlcdlp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2axqfncsv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wmbwgqmm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sgbvweqj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zclqpvvf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xiayjsum.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jlowqedx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hyzytujw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ibtgstoe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bnykrnwf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qtwikgxc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2asgbipkx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dajakhxc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dabcjebg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aklefxfu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2suiajvdh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojqqkawb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2phdkbdbu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lchpdyfg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uepwabmr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wdiwhpqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsoqfhjg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lyyuxovp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nymsxwel.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lqieizdu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vdcvvuny.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzralhxv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ruerargb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ybldmaji.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rdjcbalh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxjtrhmt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gwzzzjqn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2inlfnbps.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fgptbkuy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qjokwnic.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewrrudxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mjxsiwkg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2glnhjbhe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2knouhhhg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wvgwqveb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lahqrwhz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hrcnjnld.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ciazdqok.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bdizsyxd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ijdgwvto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yqqlkzlk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2izttfoce.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hfqlbxrm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pfvbaapt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mrofhpef.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mhymoenh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ijixmwtn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cheoqekp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzqwcbwb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2digdqnuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqqsdjhd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zfdechhg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ruidzohr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vxcgzmsa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2endnxybd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fxmbpqic.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qlvzysnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gicsuwlp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jxofsqry.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2prrymgui.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fdnrlyrg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rrsmuzup.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cuiecaoj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vyttxrlw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2clleyxav.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aiihzcvg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2smzdprba.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wxgakuba.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ypkxzzfe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ddsdmcge.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jupevtck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dxopexde.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tubrcwac.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfakfpqg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ckwqxxoj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lnqdgrsp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fowahgdw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmpybier.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ulqzvsdd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2trjsvhfi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2aadsqblr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kodvwcsi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eedzlikx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hsulazis.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2czkffqou.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gpgegkjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ysphsyny.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kizsomrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rdtricsl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ppybwwpl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xkxqomzf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2soteokwd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hrbvhvdb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nnoikpyw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pkdjvdlk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eejvdfny.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dpbwppvq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lotfwyma.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjsytvun.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2suhjjiml.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmwhxzcj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vjisparr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tbufloec.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rjtnjkmc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bqzgmwpd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2twrgpqol.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fzxqoihg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odycjbab.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mvgwgkbc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pkqbjblj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cenrmqim.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pczurwvb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rztnolpj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddofvclj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yjvwrpqe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ryhiasex.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dwosliwy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2erbcbrte.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lexdflml.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kfnpsxyc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xzfezlov.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sulrjohy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2koczvcgv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uqcahjyj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zigcovwz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ehypxrvk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2givsztgy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrbpvhc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrmjfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjthrdb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ghxoazdy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ppbxkhye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rdnlxuga.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuqwiks.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lcfwudcx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dirbfajq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2natlzynl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jepaywkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mkuilbrc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aimnqdox.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbjtaq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pvukscrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rvvjgflg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjjyjtjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jhcjbhdb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cskfmcdu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cwpvfvhb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hznvbtuc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gcmbyvhl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jkiwreff.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qxxcpqgu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsnilg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bbmhcqis.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vmnacnoe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2agbzsgrx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mepvzwlw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zkcmawmh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2notmvppr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbpvcbm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fbvynmcd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2psmidnyb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smrmucph.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kklyvjab.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2glfwfdsv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jzfxfvnp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2huuedxaa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kczblvnd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yhqeblcl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qesgvjia.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2enuoryuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sivzmfyl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejeqqvdg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wlnydqth.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2efdijmdy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tavztptm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sqwjtibr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nkquvviw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oigwlkib.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zocbfrwc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hidwbfmk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kqbzeilb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hosteouz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jcsfcfav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qbnpngdj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2phgsltjr.html


<!-- 参考信息 -->