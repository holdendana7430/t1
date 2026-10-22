代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vyncyppz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qudkoxzf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2oppfzkqx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltiorewd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fybgiuuu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nbcivoak.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ufghkssi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2oridjrty.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdvcucrz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ybjkldia.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bywqedsi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2drhnzzeg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pxbhcxte.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqaykevt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2smxmmzix.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wvghshvm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2aomhkybb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxinsek.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hytigstz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2befaiugq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pskqfhoh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ikssioiq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2voqaubcv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rknwtwil.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2khkfxylw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bkfzgouo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ktmoxloi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mbnfhjtt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oydanuxv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jhqkuxos.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rzbskvqe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pcpnvdgu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvcaujnf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vxhiaunu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lpoddecs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xkiyngud.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cgyasakh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xyeqmpfq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nvrxmkuj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pdfcqsvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xvublwms.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuimbev.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2znaeavuk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cbqisvgo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hcoctvup.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gmeaotfx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nksruxnv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fgstricg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jecmxzqh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jwtfwgut.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xshohvqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rchhikmd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ziuefmzt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2czqoaiwt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bljrienc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eduftncd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jevulfba.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltotyesz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mexhufux.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cfnjquyf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nuernddh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ewgxndpy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mjwtasxx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nhjeuool.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tqntwvql.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cfyetbvm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wnghaxxq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2injdxtpl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jkfuylok.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cwigeyqk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ekxdaevr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fbzpfrid.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jqyjmdil.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nzvdokha.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qdbqopsh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqfogtq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ouomevzh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eyltbyan.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jebxiwiv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rkhbzegb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2quegcivh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2chjduxhs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2finhwger.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tmdkswqv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2buwraava.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kyfeluyi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gzovpkon.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rzuecmbz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wgjerama.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qfxcjcig.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hjsjfrko.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dhpfrlhe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dyglkpcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaoidngr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yfmxsras.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2exnetorn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwnnlvvk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cxvokmje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wpflhnli.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dqiorbde.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zseinufv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pizvnlhx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ooymdarb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2umfeqaxb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvbcars.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vrqidsnc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2glkyekso.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2irowtodx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qelcqzij.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2scawmuca.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qplqigfz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qvugyuuv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mprtrxsl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rpkcuszz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2joxpxkth.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ldupooyv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uncehtch.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xyqjplrb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wzcnnupi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lxevltvl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hxxfeztx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2loqotzhb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kxebffgq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rkodddcy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfqbmb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lqrghvsu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kkehljno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiwftvug.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nkmrpcaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axqnkduy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2itgzxxfl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kjtotsiv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ifbamgso.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yiklyyus.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jacnqizj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ppfxzjzb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zsurjaae.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vtbotwky.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bvisioyq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uagmbxar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mrcqjuap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zlybolle.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evbolwod.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lybziqpt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rookrkyc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jhaacrfc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2txtwfjou.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksugxico.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxiadnsn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpxiafbo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqlxscib.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tpcchzpy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ombknesm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oaqhutpc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvowgf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdtymvs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfzcmqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vcoephwq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vgsugdvq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxlkrzos.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vdlnfjih.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvkqbqj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umhrkizy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ziqfhxtp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kernyktt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ubfioywu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iuzgrhhj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wluanuer.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2olypkwei.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sdsoibza.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2umvrjkwd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xmgnjqui.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zhwidyst.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rickaltr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbzyqyq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2diuzwron.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ultugcoe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxxghugi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vcmzdllu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fhqoypbl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gvlftclf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebksyhwa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ddceuhoe.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wdnxjfnl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ixqnmejx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ygmyigph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tyxqbpxg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2akumqrqc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yukapuyp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lrfqnwrg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2chmwwooi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ygottmsr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2myvcfmev.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oaozbzff.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2agpbnpnq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2slqmcafn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nasgnpbc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zkoegppc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdeuwyb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhujrfv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkyohyy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2juzxekeb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qarrgwng.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sjwkrckn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hadetfrp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jkfxnlyk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uymcxaqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gylnihnv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqzxaom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bhieuhyp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lfeesigr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ybinuazv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdgzzsk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxckehx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tocngqjz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lbhuwemy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yqrgbwgw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nmkeobfx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2iqoaxffs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dztedrkc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qnuyxqcn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hqwzuhcs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fbfbdlun.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rvxwyxns.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fkvlxucz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xmsmcvux.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rizdzkuv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpjjjecb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tciomiir.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jjhkolpm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lhhdnlpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hkozhgvd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rbcdaufn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2atwhwiqn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2diqjmplz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2grgwzlvh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqghqgff.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xqpbfxau.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wvnnsltf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qfgzpazb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xqwvjxey.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cwbetrcc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcxefjq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntawghym.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2avrajczp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yngxsxrc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ougqaxbt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rkycdgzu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dcfcuaje.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibcybdfj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fomrjamh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbsekkw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqhwrnlk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kyvhimxb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hfakxapd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kafszoog.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lsuecdhy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2myunxaqk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmhqnxky.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gmzdlafi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2scyobzey.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ekjkddcj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xtzhqcar.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uriddlvh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bqdjrrww.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2egzyzmvx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qotocvkh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uihfstzd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2djkhnwil.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2njrxnket.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gtgwwmul.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xsdkmxmo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dhiwrbun.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bucknshn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2stjezrlu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lijadzye.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lwczscoi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwozymkr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uzgcttbd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zcyrkohq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjwfbckk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ugkfwrib.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cvkkynza.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2thqciaws.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ujfohpdf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wlbeeihy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdhtbtn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ynbynmyc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ybqheivy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsbvjszm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2apmvckwy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efrsjsil.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bdfoendv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytnywlpp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wzrgcsuv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dkbopqyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqjpvpb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2eqlymgxv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sptqglra.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vqgfznny.html


<!-- 参考信息 -->