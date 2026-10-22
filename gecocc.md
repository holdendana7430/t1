代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yxxnvutg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gbyisfsq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dmhjhycm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jsloneid.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hvldugoy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pxasqmjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pcywupnk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dnvmmkhc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2shltkrlt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oxvokgsh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vunaardx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2evmctliz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tnuihqbl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pxvgfosj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2axpmjrah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uzmxjqnh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wfjyqlid.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xeguvjyh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kiumjipl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hnlpwwff.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2unsiygza.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2diwasmlb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jyxcqwaa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rxdrwdsz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yqjtbvsp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tijzkwme.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohlrmegx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qwmmbugd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qelwewbr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlcjmobw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pvgjcpgw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2huirvpsd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ullkdvbi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2awrmqvlt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fbctlbcw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2msonlmso.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2miygalwh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wwgzvsoz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2afveyozh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ppowjatd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nbuukuah.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pbveedqo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jaggapaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bmrggstd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yacldrrx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rlcfavjn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2koqudahl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2aibcvcbn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dqebmlgz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2shnnpnoj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bvtnptaj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xvgmbknn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kyfkoaoj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tivhlegn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2eskxfbtl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xqdscjzt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xejweymd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pgnddeeq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ghfpgduu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rnckkxdm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nhcxentc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aeygzdad.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2udlfavtu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kedoapfi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zxvyiabd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2sgihmpmb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhvoubvw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2quyicddg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xalxrcjn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2clwdvick.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2imozgbsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2obcrlhgu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgwzxfty.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vjiiniyg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cntbyvkv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fejemlbd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pxlurigi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gvwyntjo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zdubvenz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ubphfekx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqysipnc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukpvsjjs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xbrkrnmf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2afsqpwhf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fftqlwdc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ctpfwvxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zriqrees.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wdawfkcu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvdgeope.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdvzrrzw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2exqwonec.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dpfsoqhy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dqbggwox.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2eqpjdnfi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rvlxgmeb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kcxmezkh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jvqaldic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2spzqlwei.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fnkbovkc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tlmglovu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hpnmpasn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qrosdzeh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2iusmbmwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqverocp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2iifgedwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qopqvwzl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lkixsvkn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fqfuened.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bdmkxkfw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ubzodvzj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lqxvfobn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kzdenagm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hwfmdsix.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nnfbulab.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pfgfluuf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2utoixzvh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nocqazzp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pxedzkzv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzsphvcu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjvifbkd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwnbklra.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ddrkylrn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hhhsirdu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wctqfwhe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fnrhohns.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2otfxwjns.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmsftrbw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tiktgnvc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yrjmyrdf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2onlzrwqk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2clbpbfac.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ikyweuhb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2agnmmhbq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hcbujwax.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bgjwpjau.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fryzhnrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ypntlcgm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tivzezaz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkbodgiw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uglnvxkt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dlbelztf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lfyujejs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cagmbzla.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qnucczyf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2muvmvdkz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jjsznnhl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2odmtoojv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bqdwtjqc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sohprmde.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ajjerqkf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ksshhptw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rtwzagae.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqevobzt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjdpknzq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bcucumwq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rdgfybtl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uaslqkig.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uspcsbma.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gazjzjvu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ffaiipvd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tkgvduin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qriqlmbg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zzrgifkq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qjavakyp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnojjdri.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2onysahnm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hubipxfk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jpbekitv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zkblzxzx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uthmifsk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qdthgxwv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zjyikjlc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xncxzzmm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vtulbzeu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2evhjipot.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qhyredmk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2egbnykiz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nupoodfe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kcbjkkmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fsmpevgh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kefiprzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gedzuegi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dmfikskx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xourncwh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fajhkvmn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rhzngplc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ennxpytk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kisnampu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vajlrhzp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2olnkfzhi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xrgxxtbf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ikavahjc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vuordhfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cgfqkqhn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2iqbagprg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nnpyfltv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2weqskuyb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hixmykcw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sniywqhl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kgrwhrfg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mcligbuo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ixgngjkb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxqfogdt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zcgczuqs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jzelilzt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uzssxkce.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vmzlvhsw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljacvfee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xaeosaig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yszpmnbw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2chekuhqi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohodesmr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2arixvyly.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pjguorbl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2byzwzvhm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ktqclddn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pxykggxr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lviwizyo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqowfju.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2haznhnqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kayvdypn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwwdohy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfyluowz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2raxgfxpb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jadrtkws.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fhswkonj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hsiiuutm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aeusqasv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2klvxvhzb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kjjfnwlu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bztmsxgn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2twrytodm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bzzpuixo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pqytwsjv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozusfrzk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rnqmghjr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2srotqmup.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vdxnylqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ayatlcvq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fpqmbpyz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tqjamlpy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ysxqzzuz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcdnywbd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdyqxuby.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkppfqlm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ksxjhwyz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2khahgims.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vgseyaxe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ybhqhjyr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bfayuwxo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oedwwgjb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkknnpnl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srqxyljy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2caohoxmt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kylgqxze.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jwhuphzz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xezuloot.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2herfipsk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwsazta.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ncrugytp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xvphpcoh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wkrkgjcd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2exviitnr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ymwatwyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bsclrvlg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2incirpgu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kobuvhxw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibviedtu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bxkurhlb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmvgpab.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uaoybfdi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bruzhzvx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nworxmwf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2poalmynv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nhwhisrq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rzfgohyt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uzcjuyiq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2aembhlrf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xpmcntfc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2coafaqre.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ncnudkhr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nmogdely.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hgaeyqfe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ffgtukvm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yamaymnx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2imrjjezm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hujppdcb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2irqzwnkv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2owklyifr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssrhmkbn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxvboeq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plpscacb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkygrvl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmerwbvd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2htzblqwh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ismytqwv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yysvukfz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2khyaukxk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdmoafy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gepyqipr.html


<!-- 参考信息 -->