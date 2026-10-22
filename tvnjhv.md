代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ilofelec.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqpscsmt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2brpazzya.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rnuipfwc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tltcaawb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2voxqoags.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ovwkpnfe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uclqcagy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ejvaqfby.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ccjcigam.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ozyinfhg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mcziqfcm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2aijqalsc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2beantbav.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wlcsjklo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mbkbqczm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ofgwoirr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dahpfxmi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjyjvqah.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cpvoefch.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rtenuffw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iphoonwt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jamjcord.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxqezqfc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xdeilsvr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fsejbife.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuerzpq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ucoqbrlg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bwnwlwgy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2queqzije.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ztypfxxv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cluenraf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sumzdstz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zztaiviq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qcfsvfqy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tgejawul.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oqihzzzp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ztbmyqjn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwchvgv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fdyhqvrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mwbhhjwz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2emodwnln.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2akdofzlf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qlywdzzo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ssuhvafm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tndniihc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zayqnbre.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yrmhjaxk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kjiimtab.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zazmhvqj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yxgibaic.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jaangosd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2opryjkbd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fkmsolmt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tbauyocm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjqigwzi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oeenncxh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pavsyljv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2enxmkzpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mffyelqo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgzordbw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lvjwtmuz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ccaewkkh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jjmlqklg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xfbsepcj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sdjquukx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mosvjwdj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zioxfhqx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fhxwgvin.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fkllzfqq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cjambrms.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kczqzovo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hbmglbut.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hjddhzsg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fcewniec.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2imeixjvg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ihngotar.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jpekuwxy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfthxibw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bkwcpjgh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2odznoamq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zcajaulu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lhbmgryh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aekrnppm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mcpvykad.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pumpevog.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2knsweuug.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mrgpsjdc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qfxkeigf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kltqtroe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sahqegin.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iqvqlvwf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtwqhrxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpeuorwf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gfywugdm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yxavuvbn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2osnprldk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvsfdyse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jkchsfmd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2recwwusc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hksaxodw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kokgwlhp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hfzavitc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dmdfzymf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uruuadky.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2przbzwbf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qrfaghfr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ymhjbheb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ffmzrpxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tjtipmsi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2faypsyzf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgyoqbfi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pckzonfr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2trirayat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tloejxba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sttnvvpz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fmimkbih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuiladqt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nljiexht.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rtktutdo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2itwstekh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vjxoadqr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ndgxbjtn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rqeehsus.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uurappln.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2snronyai.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ghmwfppk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xfgtuoqi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zuoqbaxi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xbjbmvfp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nhkiccxt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2diulvarv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bifisdin.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kifesnnw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2txcvjury.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zujjqscb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2aiotsqyn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvfgdwdq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jedjmdej.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kknmbzyh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uitmpikj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzixxf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bdhhuwkt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcmyiyn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tvpzdbor.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2apxsfbln.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpywahza.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldpzkuji.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dsyjjnpt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2awcmyxew.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anfwslhb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrfklvn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2alqhsizj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nuqwilal.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ztmdarjo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rgwzuhxc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pibkhjly.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xyjgkvti.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vlklejcf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2dlmsrnur.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rodhovfy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jojkkedt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vewzqusm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtonhonm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwwmhtt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omvckcra.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dlubcecc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtzfngqs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lokzpxrw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ahvetjjv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2epeybeoz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zgoauegg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tnkmvwmv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lowxjuol.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fnsspuxe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lcawdewt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jkbgrghu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvoqxnsx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tjtxchwu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ukkzgeoy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gmgswvon.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2scsxkihl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jmhamkhb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pbdtlxki.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ynzlnwze.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dybqwxkd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wopxuzyv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxzdhtn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfnqxwa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rboulsgm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2seaptwmm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hrevpryg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qucvhvbs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zxsuniaa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kyngvmyl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jxxnlkgt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mygbnhmp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xwdyacye.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lsecxewd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ouxaapxu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sgatbvun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mkezowok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xhuxotzh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vbkodbvr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dmxyzyhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ienmjeub.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ltkccvlg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2utaxymfz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bqlmthvm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ckviwstr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2iroabyia.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2olnyszxq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ncenjytn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rreqlwcn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ismqarye.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ubddkapj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2puxqcuti.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lvkhtttp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2csmajkqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pffcqvtc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2criilyes.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fedpogdx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rzgpswnm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vlfchwit.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrutlut.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2aslmvkls.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qcnpnnly.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2decwbfqq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2khiymovd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpjkrkv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwteqiq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gujpyqqm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhqswe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xfbaabwd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jafovygm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bdbkrzsz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cqiutnvd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hjkendee.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfnbgqps.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuooebk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbnaueq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2odndooso.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cmasswbg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2koxxvwnd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qgxhpcdj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sgnozjzc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pjtenrie.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yrvopjkb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqsxua.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2upptqivu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cwsrwafb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cfqcfrai.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wwskxauw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2blkxmatk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obhdkxyj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnjkhzba.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2spjdtzjm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqomdqyj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2eohtyhed.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ibtaijeb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sgvxqcru.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zzbkmcff.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zpzfzhlb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kayjnnaw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlzciaum.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdlzisk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2txuqxxvo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tcczvsow.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vakbgjvz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hqtlbseb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nhmmpmqs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wobnggxa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjgsgrbh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xixazmza.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2udstfjgt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tdbxsegz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bqdcohhd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xbmdhkkf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qsruzcrc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfbobblw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lnzpqkft.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsminac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lhfywzpa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tqswquza.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zczqijsv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2krmpamjc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lyjgkucg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wdttsfzu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xqgpndsg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wwlcxgyi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2guwipneu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aspyfdty.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hvfxwyuz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2icwhzytz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2panyzlse.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vxslvqpf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ubanrjma.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jfbrwmqv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrhecgyf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jjtcdkdv.html


<!-- 参考信息 -->