代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yaanvvyp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qddwimdf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vlsknvzh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwmwsfq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kgtualxg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2swvkeavf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wwlsxxfx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bhpfqgtf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fnldxdtz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kylzjyub.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2avmtjehi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wlgcjije.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rfqetxnd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2erdgzuhz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sifztcyo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fsjfxegy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnptvvbj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2trqcmikp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hllmvwaf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tjsaslzy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nvasuayb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mitcukwj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tabuefyp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qseqycgc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bhihyowd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nshnhuwo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kvnqiogq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hmicvdgn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgiaojeq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dnysmdbp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvumdbmk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mbgkiweu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2aeispzvq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vwmgrgwj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lroztbfy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sptwnpff.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2narqeivg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uwfpswit.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hkjhcffb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2eyisezym.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qognxfzl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ljvcumaq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jlidqxst.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fpbyicfq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rfxlqlua.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cqmtxtnx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fhsslftf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pcjyswld.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tcsyucpe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kxpdnlpd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ptfcikwa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2utsxhotu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ikpiyoeg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ussywpww.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yzkgjdst.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zsnefwnk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ibvcpqra.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bvggnpcr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvxppplk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jwtqrnuy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eqlbqjxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiwzhlro.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ohvrqvnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wumfiadw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqohblbu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gktdksvq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nzyedjrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zhhhfkcd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yeaqfusc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wqftpnsf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xjpcyfvy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vsrqfwms.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uahgrbyc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jowpzfwh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fxnzkmzv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2twhkgzev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ugposzaq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ymswblnm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jzxprprp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2psiouxwy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bzxjvhfk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwbjsauw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uayfoazg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qsqwgoiz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xrxkdicg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gondqsqc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rahtlmzs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qgdpfsbv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zvuuuxuu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2elygereq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wbtvqgfc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpjlskby.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2klnhjutg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2leigqair.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntrnolhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfcbtdeu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yuoakykm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tobaotib.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2alrdneoz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hrzfqsnz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ymlhksnv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tjtnxdue.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ehaxrhrt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nxncfomh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmyipc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dxycxcbp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gfhdjary.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pfjfveiy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ndgnhkld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ufdntnif.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxshthor.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2envptfso.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tkrfbgsu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2enluscaz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qlqbxjmh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nddqqoew.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mbvcyuud.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vsdsoapd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uplrunyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pxzbpxmj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2toobcxej.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cmnpmwww.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2whsuokxm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qzojwruv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dcoqqwls.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2udxoykoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bewzzhmx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bhdgmugj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2esuxlutt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpodmie.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhaxqlqd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zcjhsctq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vyastoqq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bmlfqcad.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjvrvo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dnrlxybn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kchbsxuy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ljwjoypu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzvovonx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pfzajdde.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fznhtdwc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uncyfbwm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2deurmdto.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2crfjqwye.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvchoyks.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dunocgac.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ldgylszs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptsygsdy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dasrqpuy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwakifqm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2thwzbnlm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kzwexmjt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hmdvxrjo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpvcqf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2slpamsfd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dvnvzvuy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ulaelrri.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rkmttuxu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xjkxqapw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tormsggs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2svlpmnyz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hhjcmjfy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cdogzzdo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dbkuzfaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2clevlphg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xrkzrzjx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wzfdrkiv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qgmhaxbc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfwswjh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rvtajgbg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zkawcrhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gljmdpan.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywzysyil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rriawgrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xdaaxmzm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gjspkzlj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeortsev.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhbdsfgl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iaatucob.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iolobycg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2khcxiggc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2libvpsys.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dxjmncno.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2msgcdmyv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iwgyymrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2khbxhzev.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jsuiqemk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cchjqqfy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pakapswk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2licmkilz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yatjprsv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hvongchb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qsxnbsat.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dgmjoecb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vogcturz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kafixsfx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ujpzyapq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2srucitfd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ayvlyrjr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fwsexttl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aclyhuyz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yixocjph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ppqvjnxz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2llbwifra.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiczqgwk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2racyhbgv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2uzvblxdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xlxevojt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rqtthetr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fspdzyqq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fbtwwngt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sbplmszh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rejvpqli.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpbhncii.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2imgeldit.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jcikdfkn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fcvfcmei.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tkbhpaap.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqaermjl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhchumm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iuxfgitx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vbvjmohz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dguuvdax.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntpagmct.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mvmpapnr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vlfgfjht.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kcgbztqw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jremwbod.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ybuxoeac.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2frvdnvtz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ytugkyda.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tmxidahg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oitfkmuc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ubwslfgg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezannees.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxgyasxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fspoyvkn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkcxatf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2llcoazmz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ovedaaom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gwvkkzup.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sbeixyud.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iqxcdlne.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhygdvkc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2psgjifkb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqgbofvu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thlstnhi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lebfgikj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpvxgrf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2eeoigscy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ghgowrrl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2huiculbi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qvmmfffl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qdrvzhwz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2globankf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2enjwlvnz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rundridr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vlljarjh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tadrares.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbfeagej.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bkfhprra.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vjtmhmyy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nuhtwdcc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ebrqdbbp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrcmhih.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2afmgbwgp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lnjyjxei.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hslhyohw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ddrssuvc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mmbhzuiq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqggyzj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yieplrec.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sdrqdrih.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eegwzflv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2irsrmrgn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bmaohmhy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nnrxomhj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jxnwxyrc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2waplemvz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fndkkadl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pqkvzwgn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxszlznt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2miwtmtlr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgchvqp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wtgfbkyh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2esvwafde.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dzhgmarf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zwxcwdyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbbudcbh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pteozvhd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wlcdjshf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nvcbidfg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rnxxfvyx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lsqmuaxx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yohvqjoc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xevsfkyj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sqdlkaid.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mrmrbppn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dvefniop.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nqcypwpq.html


<!-- 参考信息 -->