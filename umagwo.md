代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3iraqswbv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3edyoaxdn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hmtqwiwv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nbtbkxmj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knhehuee.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bavmfeys.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxvekxu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kszinnbq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ovvuzhiv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wniiivwg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qanobdzr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3laqjziat.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ssebfgfz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gsgraqog.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3geffpgcy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vtnmiwhl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3toywdrjz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fvasybrx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyvogwkl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zitkoipb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hujdhtee.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nsvviizk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pgesqkiy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sbgazuza.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tlqlvaor.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jjlkjwle.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kyncucvx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pxeqonol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rngvtdhv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qsbjbhei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltohmvpu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oedsylhv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wogezlml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lsiflxdy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wplrcgyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yaiyphxw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbopdlmf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pnxnllab.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxqqgtqo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwhzsysn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aiskmrnd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wwirrxht.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kukahhrg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmseokj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdarbla.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nersxtpr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pviozbta.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tryczkbr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lyatribl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rujqmwdd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wfnskzej.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3usphsine.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkekogwc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrsidfec.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbcvwio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mgcospgh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfsaxjho.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ljnbpxfq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tokatgoa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nveysvnb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3aihytyvx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbnoafzl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jnozmypg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uxvwditl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mjmgotkw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3anwdzbjk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xheqhdwj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gyfwvnan.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bhutqigl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3adbyrhsd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jdxpwsdv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gjsruuqe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mmcpxadj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hhxgiqlc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3guuszrlh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kcolfqet.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3secutlhh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jlvxvlvy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vtyilmqt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pxranovz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tgiojiop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mnpggsie.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3psitbznv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ozikkdch.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bzkthbrv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3uccjwemr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rpfdazle.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fnjyhozl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zckbdzwq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxecsqu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qcilfeaa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kusslrgn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dscsrdim.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wwrnfxkw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ujgcyqpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gywliswf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3unyfwekc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jxdegczz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmjzdyk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nxekkoun.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tuqedrrk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jvhkjczj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wlkhukhd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3abtegxth.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uedcumyc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3prmiiqva.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bjultdbr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wsinqecc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3oearydor.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3omoegmdm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3odwovptp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jgyiookd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xaxwyttl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dhubxdbg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tknpbveh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3josdbiwv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbpllv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbdxmlhw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bdsqswvf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mhthxxgh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mycbnoiq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ulmedkkt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hlolatye.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dwkgzzvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3biozpjoq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yvvmnhpt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lbktsuem.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gbudtbqj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3hjsovdkn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ldkyeqtd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eekcrdjx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rixapeba.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3avepeamv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwjigf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kgtzmhdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uftsancl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oprwbhza.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jjdfxzqx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3veynufye.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mojxvjdn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dttvzudr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iiumdfmo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xckfdthl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktenjqnl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzfhvytl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sixuflwy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sszigbkb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qmtipwpb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ynizmvnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yrisqwdv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bluxbkpr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rpqreubg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcyaldik.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3syqyacab.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3njmbocfn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnccarhc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gameeqiu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3asvnbspj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ymvzuvbc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mumtqtap.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzimkqpk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbfkpxqp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3afmiqgke.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3beyabbjx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jdzkuoez.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lkbmcspm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3frlhoxzp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tqstdxlv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bddrhyom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ouxzizgn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pgnxziqz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tevpewlf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wapzjdzn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eskpviue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yfujhiug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbyybc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xsqgeliv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lohembsz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3biwurwak.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3druiukex.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ravqwunu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vvcjbrua.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mduxjcya.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3guxzdvpd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jjgnxrqt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wwvqlvuo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3keenyoxm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mbknmxvz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cmfnbfvs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3taszaeuz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3thnpbjes.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wssjahta.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vbnurjmi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgxyjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3myyaqnou.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbpavh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3szxkfqhw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpancnw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pwazxaqv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mxxoiivy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcorwgcu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3teikrrwm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3csgknyzi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmoataz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ruyxcrno.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zsnggtbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nlqqmfbx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jejuwyue.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vdysnljc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yiewtpnq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zmnvcdna.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jcmtkkfe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gskywzpk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaahashq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rrqpkwvh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iuaoevse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cjemitmr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ylcoehdw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mbpphfiu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xhkmwjmr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3buzukcqy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zbdmenuy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rqvcrwlv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tzbdfglu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmqlvhj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xnsafsah.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxiyfcnf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3crdobtgz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dzfatqpw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hljvcfoz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3florbggg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3afpbunwb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lqnqtnuo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3moqfonns.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tqztryeq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tvowvvqa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdujkoyz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fxdxprpd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wmufdslm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nlvfsgbi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3smbcamgn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ytkceanm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pmovqska.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnrgqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fupajxgp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3flsmfjnh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfyrybia.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3klztgscg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnzgusx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ispjzidr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jpuxhfpo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ztnzmnzy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xzxloiem.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jfkqytxj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nqasqihc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wabueypj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jilifpzc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vkghythl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3znjuvklq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3khignqir.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xlhjnval.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3prrpbuqp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnwlced.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fmaskbtl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lijmqokd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bmpddmyn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpxcrvy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qtanjvjz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pflilscy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xjypgqnj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvrnrvum.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fvjwjdkf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oyzglutu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uasskeps.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mokqcqav.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pjcduzow.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3aexioxyz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kwyeavyx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jdxtpstd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbdrgpbg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjokvhxr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcmwesb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kseacjmz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyxvopfw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3givfejnf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wzxqyizf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ygfxczkw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3lkuhzote.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gdsgudko.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qkcckvdq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3baiphalh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rtrhtkzj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wlfrjolc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3iaaqhrgx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3olodyvyy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iqfnloha.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpgckxuc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyeflgar.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sygobrop.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pvwrpffb.html


<!-- 参考信息 -->