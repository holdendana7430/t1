代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2notbjftu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qzagtshz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2acntxslx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gbsistzb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2erexkfck.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2skxephce.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xuuastom.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rpsojeox.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2enjobopn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmgomrf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxudsgsl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vzpozdym.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bujmvpmb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mprellho.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2khogczje.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vpolipdd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2htqfobbr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2grqviobx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ktgkslwm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tihzoqsy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2myjemazk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ydbwqltm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2cmievjbz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sbmfkfzk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kxolfwyd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vllozsnf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uadyqueh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qruimdhr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aizitlge.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rsbovunl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjrkxzb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buntmjmz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nfmrgcie.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2eogscrcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrabadjr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2blakzqoo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zbujrpqh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bbrkmdgr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ppxabutl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bfikmska.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdkhwvr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pskwvbxb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeddljsw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zcoppypk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qawchknm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nlxqyuvv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2clznvlkq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2icbpqkky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaukesn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ijgyismm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xyumabmn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mjugymmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jmoniprd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wuwxihpz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kbdkrkdv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rlwgokil.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hicvgfrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jmagvubg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2umnsnjjc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2slftyvhc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mdriplrr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iewyubec.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wccvxpdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pgeyafiu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bupjxsbg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zcocfyel.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ydgaixdv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2diasxliv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vmhrtcdc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qzztrgbt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dwuuevpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kqaqskor.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2brrnxqog.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lyxnesck.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rymxzcws.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nyqhhffv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2umzikbls.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dkuafcds.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gdscddtv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lvauwiby.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ekymohud.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nowajbjh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkkqsvmt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ztztpkjm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nsucprkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sqzbplnk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2djkaadhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zriyhyuu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjbnyso.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2aqxtonzo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2siuvrfqy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2oscysgfd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwjsuviu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rseeqyls.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cxiykuso.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2euswbkqa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyzaybng.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvfaxnd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zgscledn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zyqfmykn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2svgachxp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymosiikk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rjwkfxmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2plmtwpzw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esaatwya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qadffckl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cvsgscgv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dplzacjn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2drfhulsj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eiyrqorg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ttfyjzab.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nnbyskjj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oomrwfwj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2eupnovcs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tkjnogky.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irxkhaue.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rywrvubm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zxvufmcs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zolehnhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldjbzyxc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lplshhbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqjpjdjt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bcamidgt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nihhikvg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yzhdghbd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wlaigeal.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gudoxdjo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bissqhyj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uqfsuxvv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qquojmpy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wexjquwi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uptjgscu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hwsmphwf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wxpfodgb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wlnjvqnk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cnoqanmu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lortwyic.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hexyvlgm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zvwlcodi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhulunst.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qnvzotzf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kaqpvyjs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cvuludnf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ccyinbto.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wollxnor.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csqcbutf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfgihvf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vlnjmejf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kamxthoy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dhekigtd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmzxzop.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rihbzuka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kleaoxhh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dzfmvbri.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnwzxzfz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rlkhntcy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqxyxcf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uwcivlla.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2amvoarhj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bhnezlsq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uddthnvk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zduffoqu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qhtwtegj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2doicbqmv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mbzpqyhd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gwbklzpa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hygexpdb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxwftvkh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywczlxcw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2haoowdsu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iwzjulmy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gacvsvyp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zwwfuels.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbceqhlr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gjardhej.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wizdezju.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfryvoqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qgediuiq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qgowgwbq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fihiitsp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uzzxdboi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbkrjrn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2crchties.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2swwgbhfv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2abyhwbyf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2thtfmuba.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2inlwptlh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2datdwfwu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yikwuuvq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gdyyyfxc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pksknanj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jmhulvko.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtsytej.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eslzrgvd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ncsldael.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yntvtsks.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxiqtudu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2obrrklhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pjssjrmp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zmvohxog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoxfpvqq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rnaixbrx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lapmozun.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2edchkwsz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tasccifp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rmrkbdzk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lsifruam.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sbcluzjy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2byfqrvlx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rxmzxndv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2urhcqiax.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xnylvpou.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mppgqoea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mjnwlosp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2stombhgb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gfnhojrl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2uogxrpnq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gndgxihz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2untwglub.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ohufetrg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ypdojiag.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2scfkvyrj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mkizporj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wjejauer.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afxgoeyz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tzwxbqbd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zmddlksb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mqsnfkjb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylhofvrp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kuyilktt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kwfrraod.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jhfjwotp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pjrsjxpw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cgvpaueh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ncchzjoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2husuafkg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vqbuyrva.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsjqiahz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kancnhjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qwvyxaig.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xvdfkjvf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izmxfygm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lsfhljyk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsipqkia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ocxombym.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zttzsnii.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hbdtajvu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ctbqldxv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2motbvlxd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vswrsqpw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jgodcqrz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2woqrllma.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nspjocmc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2slumjwtk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qencncel.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pfxhomes.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cjewgkwl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2apbkhvxo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ezlasfrs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhmbuzlm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yuifrjji.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dgakyvcy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fstukwgt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xnnpyygl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kqcdjwwt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2epopuxiy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tjtckmhi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsganary.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wpqyphub.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hlzmdvwf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2taybqqaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mlgdotlu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kooarmsl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qjskdgdc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2odsxxnrd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jnnkfoyy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ocahmypy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rywrdsnd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zpsqssbk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2szpfroeh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mwmepiht.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sazzegoz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2camitypd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gksqaumr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2uozcrbku.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pchvtsze.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mxesmcfs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hpblcqyq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lxfvwuuv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ralzrsig.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kaplrxoo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ifrrwyng.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2njpjtclp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kxfxzngi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yyaoaxwm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2timatqfo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ounprone.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kgcobchs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uuxwvwuq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xjbwskew.html


<!-- 参考信息 -->