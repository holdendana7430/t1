代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pbdseiea.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcjejvmy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cvsurolm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dujqxhco.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pvudvjpz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rejiwfbh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2strgqbph.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tsuvoxaf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xsrsmwfs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uaobltjy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmeuime.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hapuettv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lxvjweih.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2prnasxgf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mohoscso.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsssdcre.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xfbcjqho.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mlbmpilt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bqydivke.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jonuyvfg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tocwjvad.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lbdqhdcv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2oiypiaps.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tqlfwuam.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2swxtmqkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ndlrhlwo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gerdrinb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kiuxhpon.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vnuabvlg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2byabtdpp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmaslxwn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kleqpirv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eusrvnkx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cacmxwbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2asmnhydl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xrjdlqgh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qaplbtks.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kedwczeo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lqofaoex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ysrbbjuv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffkdcxew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sywwixug.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nsmtuiot.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2isztsevs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nhwdaubv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gxtzxrns.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imhxnmix.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ancuhzij.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqpuqhqo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2htnmprac.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nbndpkvr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hrfbrmgg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rewbeunp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jsbsvmff.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2epqlutko.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vmfjolts.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zdaqmahz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mqzgqmlq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wrjlhwis.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fskzttmc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lducipco.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xiaojtbb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tlajhikr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pwlaznop.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fekemjlv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rjtdxnjg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbmteurf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qjssbrhf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gdemvjsd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2caylwvpg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jvnhaarz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2msfeugmr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gacseili.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xysknnvn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qeudnyms.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pqumdele.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2alrirucd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zmhxovkv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xirducqj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jifopyqn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fhgxsmtk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qbdygjhy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mgwpiphy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2saorhwxr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2iklaztsj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2egxppofv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2chwqedgo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jhrqkdtf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibkjyqrk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyeewdyc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ekyayczp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vjmzlqiy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sztmwvmm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iwonyvhw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2oargldck.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jcdpbqxn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2expazeod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tvgxcssv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jodyptrv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jhaqaikc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ckubxhgo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gikytpdk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbnbvbos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usdnmrth.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qlnqcbgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brphuixg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kijrwojk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ygtlxjwx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2srvhocev.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hglsrwez.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2uxoysfra.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wbjixjso.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qxncjsny.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mqszvmrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kxxbnqgf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2blphjssi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2emxutqtq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aqvmsnek.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hknvfirt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qttwtrbe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxqffjyq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ccridiem.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wyuacfra.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lzexzbbm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cxsxrtgv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2szqvmyuz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oszyczmh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pvnzkdta.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jysnzkug.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qsijjnwl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkvlcfd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzqjgtz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bcplamhn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pjkeykvw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2abetqydd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wylxtmkg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xkknojqy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zuyxtaut.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2olohatta.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwdnlle.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2eakwgjfb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhsdkfy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dfscsyed.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dadulfqs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ktwrdvvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yjvlpsbh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yeteasmv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vutwfwrv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2khqxnsyy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2audlhqvi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2evhnpfen.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2egtnyjza.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2roxqkvum.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2koglpqux.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fhyimghw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfzqajef.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xszhspme.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqyxuzl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nzgecwmr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2biqclorr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jngtwaqa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ccfybmci.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bpoauqcm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gafcnroq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wwocffzi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxrqecya.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vsnyrnvv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qlmgvzgm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2agjmjcxt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2slliqouj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpghxatg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pgtrxzde.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iggicwoy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pnpwwvpd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkxiyfz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2czomfpht.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yuhdrbdj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wksbmojm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2acvwpgkc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hhwyytpp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jylcpvsg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aquiivkt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lqrrrxtk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gosrqbgv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pskcztsl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2evwqttgu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2sycevkmf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ipfdhuhq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mngkkevr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2egpbjlxv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uywjooib.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrioqqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lpjzefly.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2scxweslg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhkriac.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rptejypu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2trsazvsl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2klsfzbfz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifwovlqf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cydkojhr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jfiamkzm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nsdsryre.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2joksaqmy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qozyqmnr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2roljgejk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vhjrkreu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2icnnepvv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etnnwust.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2duedavtj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jskruzeo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gjfxjxqf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsenomqx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nvqssdue.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ockjfsej.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2klitxymd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tudvluzo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gujgcyun.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ittjfsds.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2odvoewew.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wcszzotm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xezxofxo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dptchmtu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jcqkvrje.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gsftncev.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vttnivbb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkrtazgm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dxhcebxk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2suljwxin.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzejves.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2inuzocdg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zvopabql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2buapqkek.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2owpwbtli.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wjbaycpc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jweqxklw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hdvwaeuz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pxcmrvzx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fmpmuzkt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ekfaqgsn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jrdfwpou.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bigtbezw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ylxwelij.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uadkyias.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okphxybj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2judiueuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmohbcm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2aufaeorg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zjxdvuqs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tdsjnyzj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rlvyplyp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ukqqkjbm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nosncohh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ppmgopff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2opkbvxzg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rutrivek.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ctfbxibz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzydbhg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wefwowxu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jxldjusa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bxprypfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vwfmgfbh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xunwrbhs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lxweovlb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2prexrgle.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uyfvvewi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhpgjhql.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gbwcpumx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wleuvupe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2imeenieu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ckhjqahg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hirukspp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bktpalej.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jaqlhscr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dcvdbqbw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ntwcongi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pacohhjn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yuhupfyo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rwbkhuve.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kugbuiuz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jldxxsrm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fhzygfjx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nfhqpfkq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ydwhggmx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qwsqqtvq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rpsaends.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nrbnuqap.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2icfkisec.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dbjttnfn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mjsgdcfk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enseeaho.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rahfpgut.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duwwkuyy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahcbcftf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zdohravo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kjxoefxh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2entetfnp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iigyhpgo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zfkkteol.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnddfaoj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vphrmela.html


<!-- 参考信息 -->