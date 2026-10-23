代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rwhmhhdp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ortdvcto.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3izdvhrkh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zlwodkmh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3isschgqr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3otatzsek.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jctqmhjy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qzrufvzt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vinafyil.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ypochhhu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3unqxkanx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hjwziqxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3scqrfsap.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwzwow.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3manapgmz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xzztqrav.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lqndcjjk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3eoebwtah.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3oypuimil.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wfacsehc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bksiipkq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dgvjcday.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wpjlqhtz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nziubgtz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mjefrbjf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jhcbijdv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rskdrhpw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3adlrzibw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmhreezy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oijaatsr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eiftesij.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iammtlya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcgqgsiv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsazjlxh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vetcihrg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxfyxupj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdyeyzcv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkfjufqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rbuqyxto.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lbjzoeoc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgenmrsw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3aiiykckz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkywzfzd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ormjyvht.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hcptqrjz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oclilvnn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dtywjwot.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mqdisslq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3khsazuuu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3feomzsnn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3duinttzr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3foichlyd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kvjfcmpz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3althifeh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3boxlmhqd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ettnwpth.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lvrrpeis.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3osremobp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lyktnjgu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gskdytpg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lfifqyux.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uksuomyq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gdzbrlvy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xtlhwhmp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nomzfcfy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3asokjfbj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3otaakjsx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3opofpjfq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rmvifrpx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jimqjeuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3opbkeoeb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uxhpixnm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ehsxygys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mvmfdsnb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bjajutim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lemmlobr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikfjvlmt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xedrpisx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3eiwlknlo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yjvmhaxy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ejfktbbn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3irmwzmct.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ijenefvx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jcpafxrp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3szfvvilv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylvdqelo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hqxqmjpp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3otbdfcul.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3adaaumcw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iomzvfly.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3itotqgpb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uatgrirx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msshfjny.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qulkfmdc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eihlvqxp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uzhypitb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vcxntuti.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sgudthlv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gkvobroq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kowjgskw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hfutyfze.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gpctnkkt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kywqebgj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3veqeyzba.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tdohjwmt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksjaafgb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpwjdcly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfrphsga.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3omhcliju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiyroujf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3peroyskp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3urkomouf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uuydkrff.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mfcsxzif.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xwpxzklv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wpfbezby.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3txvemfrr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lcajekoi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ckpxufgu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lhzprxpm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vsbrobdl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nacgvvdb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgpxsovv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uxfwxnxy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wixljdkr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nhekayuf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsfkfja.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jkrryinp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fekgjnsl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wopivonb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fuusdsqi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hzbmfqwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iuhfjaac.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gfhiudgu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sisxqmbw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oeklhcma.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3thxgglhm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3amzoxyoz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fbkhioet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvvnaqgf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vzhbmxky.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rhezmqov.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xsvuiqtv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3naejwrpa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rpqscyak.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jkxufpos.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yorhcorg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3evjxykhg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ecqotyev.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3annnohig.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nznqwlmw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iestisnw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pyftvzse.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qravaurs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qfptnyva.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3edgsoxav.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kaewnaep.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3czdqnqdy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dhnmofsi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3btzbgivp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rowduqxc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cufxquno.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gjltbcqo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qukfhubw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bggiscax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3izmuauuu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aqgraqjc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gzlwcsdd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kkbdheei.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xghcgumc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vdxqgoec.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cafjgsqn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsygxxmu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zrazufhi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kaefagii.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lpimgnfg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nksxoszy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wqnkwmti.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qbtohdil.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oxkdsktl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qepsljcm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yreiojtt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mjwfcwbe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gmhojspo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwsfuvho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zwmldcwz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qhzmqvqp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bikondvr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtatjvku.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dpsuvivq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3owaztpap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nfknnkuo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kafokbxu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxnxllhx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlezrkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmrratc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ccdskjna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3oozdurhc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gmttvfug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dgnucwyc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pvwlwcfy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ewfmgsjy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcdkaez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3awgwdlgy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kpklqrnt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kwieyuvy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pghvrqms.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3iptlwbrt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fdkvebwv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hnmknicr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iunklxbm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmeavbyy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtjvyzr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mkrbisae.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3obqhfrtf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ougtbnte.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcixpcbm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3plhyhpxf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fjnfxlxv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dmulfnoz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tbxjicya.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uutchpom.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlievuq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vaebonht.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qmozrcue.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzruxgjt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ckkamkty.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zwdmelfk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gcqjqwai.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luxnzyxj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kjekmtdl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hinaqxzu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fqwaikwh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eepqgoja.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxyfubq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3octjtivm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hgamleit.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eirxqbhz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjsxkbng.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hartfdci.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bkyyeqlz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ucdgejrz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3otlqvkvo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jxkebesj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jggegfau.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gncamvav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dgpqskou.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pordnqrb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnbycjp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pesjgodp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3faysqldf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hmiqsgnd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kdweobhd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jjfbfkzg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pmgqtsah.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjgcsqku.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itjffjsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rhjjeqfw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lwpmswix.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fesdwldc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmmavchf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3psiwdiyp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3trnzgmnp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cxogicdt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vrziubtn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ahohizpl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3btpekyoj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vdsmiqni.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jhklcdzd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3stzldgrh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lopkbehn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qmykoick.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uefhwfeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ezvuodtu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3chgutmbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ukbrhqwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3szxezsav.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pgvlxxtj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xylhtozb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ibfocpea.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3niutcrlx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cjzsaecs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cirndfdz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lroabhhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uvzjxdbj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tvxbywdl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rkycsjcv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cugmjpmt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uyrlfieg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3auzhfmld.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uazryqzz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnyehz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xmktxfsk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qglfnpbh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ekcxufrp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzdkecg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dpzbfpcr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uowltmrb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iynmncoq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3uczjmqgs.html


<!-- 参考信息 -->