代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3eoxajhul.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hzevwuyt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ouyojhyn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pyafuywj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3iddqqtfs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dbcdeggy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wovmyrrh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3asuhyjpw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xcvdqzbq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dkdhshbv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oqjsbvwz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nowibces.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sieeejpt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3naquyfws.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ktpiyqud.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fiateyyw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pdvfoewg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3djvlrxax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bovwfdya.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3takjhlmb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cbtbbvfe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ptuutlzr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3djrrrqoy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fpqbpxin.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tpmiftld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgppsuhz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tijqkytu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nqcayrue.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rrcetmoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3iqzmmnjk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iftsqarf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ehwuefrd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwzttrt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mxyadhrk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3csjuhwmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hwcqlrza.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3isqgkhit.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnyuwhxj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kgqeboxb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3votjaips.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knruuaan.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fdzmwauv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ywuprcgp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3aovlfwpf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lcnubkeu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3whyybidv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3toxfchol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uhesipnq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iojwbgkq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eumkkcer.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3udfzdlvg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3labhiywg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zsqztpun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ekwqvloi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3blngxywo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wkyjelvr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rwkejcgq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dojuiffw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3arumookd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pzwoslrk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mrsouijd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jvszjqfq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aixkqvqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cmqghtol.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nikmqtmz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3onzfnnjf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iydahquj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yuhjjtsn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aacnwzjr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrutdyjt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3axrkgiyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwvdnpg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aemeigun.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uksfztyn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jhyavuxv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3chwowibu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dmttlgnh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3iluetrku.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jtyfxgfg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nnkiqher.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hoarvegr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hugpddgz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3awlarrhk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3loiyujmn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mhpoqtqq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jeowaovb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qqhpyrdl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3utbfdijb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfgkyzyz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzmpizkc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jcdukghg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xyhjkcdf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vfcgxneg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wdzslyup.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nhcipekf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ptmaegkp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3djubeuka.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3shpwqokf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pzxrefhd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcmqelpc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3itkjvikv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sanvdwjq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3iphswwfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxqaqzbh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uouedgbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vczokbfy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cepbfvmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lpnxlpqq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mlqqydwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3chrphybz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3esvrcire.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vdripdvi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qjopipfe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3efsyvqhi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ocpenqrq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iynfenhs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cmapbidw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mewqjdkm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xlpcbssn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mhlxwbbl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ffbbbmts.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxyuarq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3spqpidty.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hlglznrb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qmubgdxe.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwpxdetc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jeaixgpg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pzxurmrk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nsabrldl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fffbdryo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rucwesrj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uqmbvzop.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ejtzogtl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bbyxvbgx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtnjiok.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zzwqunvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3atxihbio.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mdjffruc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmwkbqoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nvazuuog.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddagvoyw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nnbnlany.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fhrrxxxi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3znqrhaka.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iczcboef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vjposkxg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vnaezazj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kbdpftji.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xaifjjvz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3siuagngd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rampbivr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nxuslzcc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3szmlejwe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yziaqjiw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ueltgfal.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bapcgmag.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wvjbmuhl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzjfwwb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mfsdherd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xxjkxoee.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fmxuqpsp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tjugxiwf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlpbrylw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cuicwfuq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vkxmqxee.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rojcsais.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aqagjrlp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3okwyjzrl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3icslntqp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nqolhdkq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tdilqddk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jrvkzory.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3reddaggg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3atewgclu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmfxpxll.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rhveeqgo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aazsnhkg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wxnrlzdn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wujflssp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sphpdbhr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhemcies.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3akryybwq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gmmxepoy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3crnkfmwq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqultdru.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hdsxolcu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gbggiwus.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gtirzkxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iolvkaes.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mndlxwms.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwgevab.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zwehhhdy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lnksgxye.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3iknngxri.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wcxlhmar.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mkuuwvgc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3clelwqwt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iymnbhfl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3syfyphsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3epbqnell.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3guelwzzq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cbqfhoju.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttupfjoy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rklxdxpu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xxnojfcm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hwdxevwj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hvngunjs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhplvwco.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rjixknez.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3semecrrn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjgtsmf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkdaalac.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3whrsmuch.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pieorham.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tfgntbxe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3osbgwjfq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uaagvhvh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upaftccf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmdzcsx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukhagcyo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ikbkmipd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gdmwnllb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3imsoztdn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3unndfqhl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ylujcpxl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyvclksb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3deewijog.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3eggzlchh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plrivvpk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3faabgppd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nnfjvklq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nanzkhpg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ijbqpvge.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tqppgety.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mkdoclqn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dwzykknq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uwzcrrtq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xxgxgfix.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sfejfsbc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jfhhzbzz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hprdnxze.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bakfuxir.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdlrkyb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkwrdfps.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uiuhfahc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bksjrylh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ffkuuegy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ijmgzeju.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3opztwvkm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3aiofieik.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hkqcinpp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3trozszcr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nyoinmlt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yemkopzb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztcvmkab.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lswrfplb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbadbxnx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3iflvcltd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qocvqsrg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zlvqdpea.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3najctxih.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xpmvezit.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uqtmpenz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yjbuemqb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tfavjgkj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ffypdhym.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jvvvkklb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbhpblzz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ebdsuvar.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ujpshfwe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rycqxuhc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gjsxflia.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wdehnjvx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3uqpusnhi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nqkxiwxy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ijptlgpo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dkseanfx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oacxnleu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yolmqxvb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvtgqucz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vbhuxaxx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rxtveceb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qopaygqz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bpbfapin.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pjlgqbbm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vpjfuxfx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gvkrulmi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ipgqwhwn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qtfoazkv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ircjmzdi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yejxzcmp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hilmkvtj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxmmcjth.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hqraniyx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pivbbkij.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3whddjvve.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ruaufkff.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xkulcgxj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kaypahww.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hqvvtyyl.html


<!-- 参考信息 -->