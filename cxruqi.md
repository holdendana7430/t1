代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tmusstyl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mdbtgstp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pkpowpba.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vaaobhog.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mnvymxej.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jjyqdlcx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pwaslwqv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tfpnktje.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3awdvonkn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fdkkmgqh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gmjmvqfe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmpfuj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgosnhj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqoiro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kckccmdr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vhmgtfiw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hkboqxke.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ulerhfhw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zzfezcsd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ghjanlnh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3huxnarxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ioqgehit.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iakiagjz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kraqdurh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fdhnetwl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jsgevhbj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eupkvlor.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3trmppogj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cxjrijoo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lwdpueyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gdcsrhas.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zcoklmff.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3smhfovci.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgysyow.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qntkrfjy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqouzqqn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3foxchety.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3utzuuzbm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gyckstvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tfaexnra.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yfyispqj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugmpqyli.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rpnuaqeu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rroauwlh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qtcqvlxg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dkftnzmg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vatkosjs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xbkkcrox.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dtpltmaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ynwolvqf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ayoogifs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bzcdvglf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aeggankp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jonicdag.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qfpeaxnd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3oxgwxcpw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ukblwnzy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jppskgdr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jihhtnuf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3emjdujyw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tjdirdys.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zpwlbtnk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ayxesosi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3duuwlvco.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvybjqdr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mjbnwpll.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gcawmsts.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tutqkbhu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dcalktdj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cxxobghc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hmfazopn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qytcvetj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuxsscls.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3istgrxaz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3afvrymfm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qbgqearn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xewvogqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3houxnczx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3emkwpvvk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kydhokya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3herlomzr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ccyhgsat.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xtktamqm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xmotnxsc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrdpdeuw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yvmqmyoe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xvuajfyv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gdoxxvjm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3btdvnntc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ryxprsos.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hlxvognz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wiwjcmba.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ewlujgll.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3szocmbdu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3biawlyrn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqrncf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zgvjdypw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjrbkktn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3errkuzev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ookegoks.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3revqinnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwkvlsmi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ztdepexr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pprcmwbo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pbihyzzp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ygztgfop.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3doyfdlfn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xlppucqt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yehrympj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kxjclqyw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xozqogyg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kxnscukt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3igmnqpdp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kzfwvtme.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ybtwtcnm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xinmrons.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cyncnvqg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zfeaouah.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uoqxmady.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3widjzgwx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xgyvuasc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aflwnxze.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3imzronsu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tuctrcni.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrwzreb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3irvudqas.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mefkiqbf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3aebjhoky.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kiahiywp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3umwxxoik.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozllohnn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3limvmixs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fpfchlwe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbcdyypx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dyjtjrbt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ljtopzah.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cusnntlm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubkmigvr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kuqvhqie.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uugsiqpb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uihlgwwg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cvwofrvf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3oofnztec.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gvmirnfl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3midcfnjz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3plbrpdak.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wyumvely.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3npunpvoz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lguyqizm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmqcmpf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mjiehrti.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3njvnntus.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wtigjifc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvohrbij.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zkaenyoy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hamypkrg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bdvpbmdz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tkmfbfyn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3byxprcvg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3woakrywy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tzizfcuj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgnrtty.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3otjntrll.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cdpbdror.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sqasdbpb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gtxdoucg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jlibgpld.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kdrcmhtr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3divubkyq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3joelvkri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cliguuxd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3noujbhew.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uoguzehu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hsvcylqg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ahuhjmnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ikypikdn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mjuzesbj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gubvxtno.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kolfcogu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3myelmajg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qgvaxcwp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmtimz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gxqqzymy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mkshgkjo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zoexuitj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kwjybxme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3svykmonc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mlifkkld.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zmntdlsa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mnsffazd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qpgpfwcr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3csfskqwl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kvtotlfb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wjsfhpwa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jydrrkha.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tzczcrau.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dmptmqxu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3oojdezim.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jladsavn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yaxxwuom.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3axjeaizq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wshhwxuo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fwcybkdt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kbkjeake.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3laiggovi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdrhmbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wygxgdvs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ksidcpcu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhrtyrk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iaawogol.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aqbldbqe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hygctloy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cqvduqjk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzttfetb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lvvklcam.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3trakglud.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zhdtupni.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pofynqqw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3chiaapdx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jxhivdbq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wsqjibqu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kncyitpi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxbddda.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bznpavzv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fequkuhq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmbrviqs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tkikauhw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3usewbkxx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tsjrqdpa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zmjekyfj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bsqeaafs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wyjwagwa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ghvjzacn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kvaurfvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dogcjvnc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hluneurm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pjpcvbox.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ykmkureq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhnvffts.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3plgggjer.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nifhdngc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsfyzpc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qfvikfzd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fflampap.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wqqtnruo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mhqwpwce.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mjdkzguq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3snczyxhl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwiainkb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yrzsvukg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ssbbfgku.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3scjuuohq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugydsosf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xxhvarmi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3devjbydw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3erpsvyfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pfriysvw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vwgjevsv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3msnwobio.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xnuliadf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rogbhgkd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cjojogrr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nymziaeg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktudvbut.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ohexhmye.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mhbqriml.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tzpcgqde.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rdjpqnio.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tzqbdhrt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yntgodbn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3kbjbmfuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvmwyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zdinuolc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uqagubia.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jogiqnit.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mklzkdks.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xwikpjwx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vtbkvusk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pqwrmsvv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bleczzot.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ntdpgpfh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kmojatyd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3swjmesws.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kbhdddfv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hhfrcdmo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdawsrj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uwuznbvu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wzhvxjdl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3llxsfadf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gqcvuakf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqyidg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3acnwjvak.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xeomkgsz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bftpqhaf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxuzfi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xhcozhbj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kxttzuhw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wfilzkfs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sdouzlnq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3neiyqnwp.html


<!-- 参考信息 -->