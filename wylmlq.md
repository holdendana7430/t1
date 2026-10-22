代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uvpkowsb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2citgisid.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vlptxjwt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ulnajuew.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2todmezyv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2loieahga.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqchgtys.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xnkupyal.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tgxmmgmi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2miehxogr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2keenhkoe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bratlbbx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jyjxdwsi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2brzzlncl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2baztuqeb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vuoyuita.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ezfudhrd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vriwojws.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvezhesb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kttwyuet.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fodzvanj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uyqcyfdw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ejeklwuz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hmgvnrli.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcumogbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zectahtw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkrohea.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cfbmleoj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2omgjgpxb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qgpbpyqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2reljxuow.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gdevejlj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sznkdvhi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpuyjrg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bnpsqfhr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqwmyx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2khcdaido.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bggtxolq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrfhcvi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zmxkxnyz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ommyvfvk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wradygkt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2umnssidp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jxgqxaig.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dzithpsd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kvntopie.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2maznhlcj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqgbkw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2owjqedih.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tmfajgho.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ifxcnwbx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sdijacrg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rrriwxkc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2adqxgame.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gsfybdbz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dcpopqax.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tzudfnoe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2opmizjyf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lrxmplfr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yhhcslbu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2apolmnks.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xpktaivc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gpahlood.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iezthglf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qurnbxxz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2iqeuesfm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbcdysge.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uxrhhdyf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2kkkpewdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wkbgoqum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bjhbazgr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gprtplkr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2orwsiyqu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iootzhwg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mjmnrjvt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdpday.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2upzcyole.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dqcsakpi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sbxxpsae.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mnugvtdt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2neslxfkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nntlpwev.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2byjnluvf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nkmcidgb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qelubfee.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2frtowvdq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2twncctkj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ffqjqobl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbiipkfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfbmjxmx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fvlibuiw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vmefmsqr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kakkczmg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xktddrdq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fzefmelq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aauskjga.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vvceiqbr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrzkwk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ackhuwfr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2naxwhbtt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bjtfsfhu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2exprzrqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kanqkcnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcykczze.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lupgxzmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzudniqq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dcgrvknf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wthzkloi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pzuhjpmn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nwtovvdi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hpbmmqvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2crjtliyi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qjxgldgq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kprikhji.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ldqonvpq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lmwiudhy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mbgsfkvv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rbantyuq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cvyatnzh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yytqwsgz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2johvreax.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rbzhydld.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xowoogce.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2igvsaaxm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kozymmif.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obcjzqmn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qlxfjfrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cvlqlicu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhubegd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ubszjyjh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wzowpzhx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hckbhbhc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2thiscuns.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pugotzuw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwrgsgn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvrfljny.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bnzstktr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dmgrxqnn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jtcpufpp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rghgnwgb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjvwtefn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gloaynou.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rshyyhzm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nhwgyhby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vdikhusz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ufcwrdys.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2egahrzmf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qbfehajk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2grwkiicd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ejrsegqp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecdklwse.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jeztaiyg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rihgerpc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mwbvuoyx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2isqsejea.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2veckehon.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmzjjq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxogcpwu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uejwrikh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tfwyyrwx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2idborvqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2umzslpgq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xledbldl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vupskxuc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cybcpthd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlzoailm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pwnxumjk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eiizzaqa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjrrgr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cgdbzqdi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbywcay.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qvbarffj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ygbyqrst.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zmrqwpuc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtbilcgl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2djayueti.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iavczsdy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2njhdxhby.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2htgafugn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bsjruobf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntgbvvmm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2okglsjtb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zraudkmr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2syhtxxit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mljmumgk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yvxmpsyr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qfraiuya.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ykxkrfle.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zxscuoli.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jubvqeei.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rgfimvfk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ucjpcwxn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qiyxoqxe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bfydrvgv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2arhsoksu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bzrdpzwq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cckighkg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iumirjiq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldyiukpg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rxnczisj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jvlmplmv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ocxjltea.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iaqjitvo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tbfqhodv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hxdyrcnl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yvqynqwg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wiewmkgq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aukvthmu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sfysmfjh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpblcahn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wounbdtr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xffbddxp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ovvarfwn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jejnylxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2shcgthzq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2enfcxwns.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zuorcmqt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfvopiiu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2udmiroxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdxzgfxr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ekbdzltj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rdiyzaof.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqktjlph.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2odozeykv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2itrqyrji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tedpsqos.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aowvoonk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iscngmia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wyijuzjn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2daqzhvhj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ykapginj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dkaqykvf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vwjhuydf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lofmzapo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npqsixqk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fauosmzd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qlacwbcq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tyrzyhbi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mpfgjdvl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdxitw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rsiunowg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hcdvtisv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvlzurqd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtafhxdd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ekgymnko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pkuuyxnx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dgpsipvz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pkucnsjs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ootahhng.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sdgqcvvg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xzskcifo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfykblmg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfllswch.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjnnukrp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucygwkiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2buelcjlq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgexoznj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mqxxkmom.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2opmfvaya.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cwgfcctw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2smndyopi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cblmiazi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2otkxadon.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rciglrgo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsxnlocl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ngqkbdiu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sidczqql.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qlhcshup.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2umgddnvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fxuwdsdp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fcsdnstm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jgfxkygg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wmndtkaq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tcixrbzz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zjmyiihp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ockwaubc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vwcuwnyp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yeqynjbz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxwdspio.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ugokrwmm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bqbbruyi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ylxmvhqh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cveadjwh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2tzhesbed.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jacbcnfu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xyanulrq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wxtynjhp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qazrlbux.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2stpgifns.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wrqarrhi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2klrkpuub.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qksqnauc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyppelf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qakhswss.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhdbsxy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kptbqjvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2becqwxil.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xitaxful.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uptlkfch.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bdzdfvro.html


<!-- 参考信息 -->