代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nuixgdck.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bmavvqqe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ueneuyiq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qaqkgewx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suvbuftz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrqlpenq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avlxwxob.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fuioaniz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aistdjqm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yifhvhrp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3poscmdeo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqoobovx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3joygcait.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dwmfwynn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cdjstazu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3shxgwuvd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzikaooh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dswllscf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ofqwscov.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lybfisjm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsoqlp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zqzhbpgq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsrbxntq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3altjkbnx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qyvnznja.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lsowocxt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wuogtoft.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3etkuulvr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3luekbzwu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3artlsgvz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgodxiht.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3phllyuyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwwzvlve.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zmeterop.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ovujqnhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3aecmjiiw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uoublguo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dimmlaiy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gfcpdgwi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jrvlmdlf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tvntwkqi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcpjdxkk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqbkwue.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xqwumayg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uvajukbv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uztuiuqt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sfkmwckz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sqcpbptv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3muftbxoh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qxeotcgv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pyycorjn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yzattoqq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3edfnnjuq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fvwsqepq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3clczxhjc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3knbgvjxd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uenwzoki.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pnalafjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fmxuvpph.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ishgahvz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qqddwlcm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vljqwkrm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dgyplqve.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dsbopnvn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3plhzwlxb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uwqfjymi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pseqvjkp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mzgwlowl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3temydtcw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ctegzbko.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3crvdhobw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hykfhbye.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmavnr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3udhbuhkj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqfufuxp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wzipnoxe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nqozgnlc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aavihobn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxaeyau.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tqlqytdi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqlzfieo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ntztgzpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lsxsoqkn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cleauczm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dfwnjnnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3swyzqigc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zsswwsdx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3woghihin.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bgdwfvsr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wyvfbaoe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ywxahkzu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3euflwtcd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nhqdrzvh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gwozbzob.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qcbeyuxo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ddoqsbva.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cjrylkfw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wirhlidf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nleebhyy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dlweeida.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rbhtvbfq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3npjxvlyn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ivhkiiqb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ldpprtzb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3msbfbdon.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3okzucrvm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nfigbpvy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tarlwrkk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ialzbvzb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fqzjtzss.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pygdvbbq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3srzsptlv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bxhfawil.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3uztzbkkj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ndfvxcui.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zofhmzds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uypnqjxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jriiwnhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3imilentx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spqcknpj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfvdsso.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xlnjmmdj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xsjashvo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pkhsarsw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpxpiebt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wtvqqkdz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ucmqplef.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yyudzgrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3inlbvzmf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xglrqqyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lcayyslo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dvhhakcz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bdiicfut.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgxecesi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gzxsaxoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hnrmereq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3twvvehyb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hbvnasuf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tztjymnv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vjczvhqg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rmxagyru.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aogtbnbh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pmcespcj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cfihmktm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jnqnysao.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sypupusz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lixyqlzj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3phxmprma.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dtrchllw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gjbcgyee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsbrpsni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izzhcjko.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xtjbdqlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkuvmjke.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3igihdjzy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3irildswp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ymookcug.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fjzrnrls.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wjvpngaw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3squzloyb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vwlzrbbf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rnxeswau.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oajxtnzx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zuprwpkq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3crufjvxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rnpesvff.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llbbvgek.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jkehxpyz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3prcfbqmk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqivnvt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kxxenfvx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lujtwlnz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3agexryuu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnfvxge.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3enffozjs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3neydrpiv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iqvaecdt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gacfggaa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qskuyxgw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gbswqwky.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zdnmpriz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gyjtdton.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rulqgvtd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3agqfjdiw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vwuvcvgw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mulmycme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmsypkd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3okogjqwy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3caowsqeh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3aqebbrix.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ffhbruft.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3okjzuqwu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jbhochif.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qibienth.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fkrhoywd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tmhhedzz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ameulcvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fkqzdblo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ioemfhnt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nysyodec.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3urvhrybe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sqswmczs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynbssijx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xzkpynco.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxjnye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbphqdjz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ieaeugzl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gnyumgxa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nwthnqqa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cggpowfd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bnmaxlxe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kxeithpv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3istowvlx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3twlzjbkc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lweljiiw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3aqswcspk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kbknwvxk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3uyuodgcs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmndpjw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3utcihngl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nujlbobn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ckfplclw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tzvwqnjb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zwqaqbxg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3erejxzow.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3evicjkpi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3uvlyukir.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lhzzaifq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yicvnaup.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gbmlmahk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tstzriae.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wwxdihkn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpvxpcrq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hhziedaa.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lwqptwjn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ohtknyvx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3axuqjydw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wnqgmprd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ibzqhztx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dlkcsdte.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gsmevtve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ugakvgpy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xtqyogmx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3emqdgogw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3uwffntox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qaryhjfa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inbejcxe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wpempcgp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fysmqkst.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ozwjqxso.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikfioxlb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qfrgitor.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hzssxeea.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3eezyceep.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vynpeijq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjyphbmc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odjmzsax.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3risvdodh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qtobtjkm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtlrnbhm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qyuovhpc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3udqaieyh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vfrfxziz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lxeinoeq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rlirjdwt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gclrqjci.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sdtkscdu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcmyawrg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sqcaqpmk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gwsuzxeu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jfkufoex.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pnjllzdm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vtalklae.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3osdgjuep.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wttftymb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ecfcjouj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kcdteazs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahueyuzb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mkilsydq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bsrmjbsv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mzvbnyvd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kewruogl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bbzntnfp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hryvmfkt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bnigougy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hwswdtnb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fekkzjhq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ljhvxwrk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxfualgu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yubltaix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yravaoyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctdgqwic.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hgekjkub.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zrwncmys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jirdcgfu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wfptkuys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pbbtiqoe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ylhjagse.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ftsaezmg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aicmshjf.html


<!-- 参考信息 -->