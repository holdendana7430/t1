代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhpqdf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lozheozq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mnwkuhqv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dzparwgt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zlaybpuz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ipcpzpnr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mqciqdcm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrakfffv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hufiagdi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxalipu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yyrjbxce.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ppcarlmk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gqwutarw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3haowasko.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ysmsswox.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qceqtmyp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ctpdugri.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvftrev.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjtovtzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3irroopzb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qacprnwc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ojyvsceq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrfrigt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwzwvhmd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tybnzimf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mvtbvkal.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3amonxffg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pxlyqxek.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eavhybjo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3urjyhijb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcoxcadz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3prmgvzqr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ewuxudoe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3behganaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dvudxlaa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rkvjijah.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xdrcydro.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sasmpfbq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kxuweurq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3knwywfag.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asihhthc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3exiwnlce.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zegtijpn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vsijlgcb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3knyqwugi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3efqrqxyq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pinweymv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iyckisjz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ekukffmq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xwqmukma.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bbtegffk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ymygixcj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vawvfmdb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mszbruwa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ukirosiu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wiwxaaaj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bornhpbs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3obneefru.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ycoqtvon.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3weegulyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lxdrzmkt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bbtfnjcv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xyvyjynp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kgrlygmo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxjrqxmi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3goqtxezd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3opnjpqnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3oohbbuwk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ecickqws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eknkgdiy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3victsbrc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wckpakun.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmkekfra.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3olomxsju.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xsxjpcmn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sriraqru.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ybcigrbg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3njhclscd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3knassmwx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kwrdyxuy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lpwllaky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azlkvrhe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ifffxglb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3isaihfpp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mavavaij.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ymnrhpql.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3izelsccy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fvggzudd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3egkzupbt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ahaoxgmw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uxpvxklt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vttlqfww.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ccgosnfy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qqsubjvd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xbpgaudy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfarexxb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gvjuvgcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnmwkijp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jdjwkkmp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3raumdvws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zxtoiekg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vysndata.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ppvjxsiw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dhortbho.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cebkyznr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yabknzhv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pwtpnupf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cbmzxgrw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zqnknghx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3terbhprr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cvnvlrtf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hjtquldc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wjabmzwd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zluzmxqw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3atxqzfxp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wudzuter.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gxwifiux.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zrmadoha.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tmhheyng.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wljmczlh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3valxemkt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mlohcrhh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3khbmeyit.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpixpmw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqiypk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mcvxeeqe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjbyjem.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xaalsbli.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qpgqwfts.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3imjyfror.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ybsdtidq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rmfkmdsd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jbslbwza.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jixylpci.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hvrucwdk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hojpecfa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3izxxsoic.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cgdsfkob.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iqwocrfp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ckoiuwiq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nnxjfqzt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nniznosk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dwxihcgu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tjikdtxa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfifgumh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wxkbhevu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vaxsgjvz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xykfomrm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fntrmskj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvdtlks.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bgocpfnz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cwispmzl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yqkkduar.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xhsullzt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vzquiino.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jepweftm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdjjkhln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eqsfptxc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bxmmuzew.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cljnlwmu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iwtwixew.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3upmfmoav.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zisismmq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mfgpdpjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ncjfeykd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xwcsbfdz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kfmqalvn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ciccrlqf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3anivtcdo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkpraoit.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xgaufhwf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wbiooade.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jckdfvvd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3thzveoeb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bdyimaye.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3abgjgoox.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjheeola.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wprgkndt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hqdqsygw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jvrobmhz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3luftxxhr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ujetqjph.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rivfmvne.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxlcoky.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eohogoup.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jaabmbwb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ovpasumh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ufpdiopf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jubnnzig.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dbnncibr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfsqwlrl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hmuhpcoc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cvgouimc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ypkufcfg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewemkugg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uinlplkx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ferfnosq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gtidtjqo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qjkbdxld.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvdrgbpi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jatbfmji.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfuljajb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gsskqzos.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nofmcskv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxjghoi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tskfkrnc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pmnspsji.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hjfkvfic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lleqzesu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3orpqodqt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eflmbwah.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqwoljfb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3etoynkkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wyvpblqq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rrpmnlkz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dcaakonh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eadsqodz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehkdbkrl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtvrtsz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yyavyqgw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ctwgtnca.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nauyopqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbjjoev.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tviybrqk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xtuqbihq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3edfyffdp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3taufugrc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jghmhjhm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bfuybyvt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3syncwucv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3oepebqnq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cqvhsgwn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lsnnavpv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cjqfczvf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjsasxt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojmxjlln.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lpjlwuho.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qxckqmmu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nqegkbrl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rlbgoywp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gyybryra.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3twascpnn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3htfnaewl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myaaykpw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnuveswd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywgmylve.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3spnxonal.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqdgfif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3izsyafhc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ydhoiolk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fqtbitra.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3olddscri.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ebwoburq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hzynkjbj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ochzgsmm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cnqewbpo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpoqcbnn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jmqfnsuu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3avfsvqcc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lyxopjak.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ngluflka.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3geidgfch.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qgocnloc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ebxihuld.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mneimxlv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hxgbgirn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hqcscnce.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfxaoxz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gsnzblaz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bwudcqfs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzqkpuy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nuzfswza.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nxdlgszh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ikhufgpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lldfwdxm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wtoorywd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qcsqlfjk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wqgquctb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wfibcatc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vrcqzsjv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfothfgk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chrsjsgu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbagwqw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fecgvhrj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jyhpsvcd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3biidesly.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ipnhmsvq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ajrvkfsf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3axvbuonz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uafwluzb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnhwtmfc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uqnxbatw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrcvocim.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3suztmdeo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dajjimsf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ueyyjvdw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bptdtnrw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3blkvaeuf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rbhdppab.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3datkrpzb.html


<!-- 参考信息 -->