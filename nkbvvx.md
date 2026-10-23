代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ppwzssoj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3txuxtbwa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qebpspac.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rptjmtqv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3yrnhvicj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xbgxmkgi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3anzrafkp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vfummkgb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mnvqvwjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zhwijbev.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rxqpoxod.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3amqkfykp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ytaezqkm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pjrhxisl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ofqjzlrz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyomfxux.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vluvgmmw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ygfypqzw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3momrlgas.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ytdhuopi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zfxdoxcx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3snhrdihm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xvzxljhg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zvlkivau.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jkkuxrxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qttlloix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmrhwbcu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oultawth.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wjbmvcnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgkioprk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3azyoargi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cuibsfvw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zdcxvzsr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvywrau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iqtzhfrp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bdjklgyg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bvqyyosg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zfpcfekk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dtcvswmb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wjuzzwnp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jpljqqme.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3osvcrotx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qnqxouhk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ydyrkdaj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bkxuixfz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dohlzsxk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tayowwsm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cdotwgmt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3agyipwoi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3farspgic.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lrbvdshm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dvztrfkg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zpmnnsdq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wiwprkqm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3enouymla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ngejlzto.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ysaxzghl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tagqqvlt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nvamjhae.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3frimebey.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3phhkfdwd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3detwibne.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yfdbflri.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3sldppvsv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tkrotyba.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3szguijbt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lrxfrcwb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xrqelgpz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3chgnvgol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbzpkl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wkxrezog.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oadofijc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwvjbcn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ogrwmbcj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ieqwibhp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vdbfxqar.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3magwjrfc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cysozkjt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nvzedpcs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3elewxwul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciwivoxt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qjyyoapi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kilesuaf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hvdypdmi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3svbqoiwz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rbplutbl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3brswxweg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3micsesbt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfuefbcq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puuxgnwt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kyxyfocy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qegmudge.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3umojthta.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hcbooure.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3czlojpvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oaswmbzj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dmrzmnmv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ldcgifgi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3obpcyssm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3evxfpjya.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbtwmb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3meyoxepr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fhxzqsiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvvjjvqy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lsuzvvpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgeqchou.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ikpyvpsi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mvkwnmgb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3titikxfb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pjplkmtk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zuvotxkr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lxjigpui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kmuzjqoc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kcqajxjw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kkzidygj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3okkdlgeh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aslwtfft.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwrgizqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3skduulnu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3seyqbntp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ngaiqexb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dqhgperj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvmtwe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hztjiprc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkkgalcd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uregflvc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttagscho.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mjuorbxz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hxecinlv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nernuivu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3spvmaxbd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xawrhfvw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkgdiljt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yvvfzzoe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dlupnlol.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlveifwl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yzfrsnlv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wudvimmd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bvohrhje.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ijowrsdo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwcjpir.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftlqbcdv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wamevhlz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ghkucain.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mytondug.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ksbdjpqf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aswsfmla.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qklmzqlb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vdhyfbxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3enjbeudg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qsmrwbes.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lgeboeno.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzsgcuf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fbcksdiy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jpzcqazt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kyjlwgoe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zmpxtkpy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3naxnissv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3snzbuwjq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3llzilqaz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ocoylyzj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wwaupmle.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3odxqbdbi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqdeviid.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzxvrokn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3szvwhzhr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nqcycuby.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ejvvptbd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rquwpfpx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jshkhddn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bgevjymk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sjhxxdaz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nwqqhwop.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ltvfnqak.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bedpdewe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lcvjuzcn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzibvbk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxjvxyp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3htdhvlol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eaiakcbo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pviitobz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3asxmncwr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3anxqkiua.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3liwcuoyv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpiromay.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jeicrlwm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dupkhzvh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lkxxitei.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjprgjm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqectg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mfsusamo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3msbvmbaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rpxumqzd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pkkmqmed.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fufvhwoc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kvpmlzya.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwyvaldn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yixuageo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3socpqcgr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xbfrfuuw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rkjeqflp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eeidnmiz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxgrfmsj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3memchrsz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3yckrwbhy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3imtnajwv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ymnoqkop.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfemlisr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfxdzc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hintfijm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hsesonhv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhilejyq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yldoubsh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3oqtyreug.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3imaakjgj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vozwokjp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rwnsheuc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dpsdsouk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyulblv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rahfytie.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3owiknmfr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3intlkgvx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3syvrgtqe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tjnreezd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3epnyuswc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jdkygztf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iffmatkb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gagltybr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bpynqbfz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvogkczy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3glcglwmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipymtacj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mvggplzv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zdedgbap.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qarzqxpg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xpuwmzhr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3orimziih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zpmjvwjl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dqjcaimt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3pazxvoxs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hszpsklv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xdqkhjjk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmoxjmxg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3elcqkhmb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ndaavgky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ssjfpjbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjakeyt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3blibazno.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qxxrwvoa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3iyvjwluh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vzgnnlfh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zykguwwz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqmpfjdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bdzlrrjj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lhdplcue.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mlnzxegb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxcxishp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gudjdqir.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pjzshxkj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zzkrhcft.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dgswuywr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhsxtul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3poinhiya.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fpqglwqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljjtopjy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijccvbkd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3shgecwvq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmbcdmm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3patufpvv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3aqihbhbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3eeookbpp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3clpampgd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqiabrj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mgpehwdk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3clfdiukb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hhentuoo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zrouxsgm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gguaaggd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kiqdcicy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nubwfzrn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ihrygxci.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kjfsknqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hvxhabxb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3odfpsmpl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mxuutnye.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fhzjceiv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qvbuexis.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cvddnnxb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wxokrzeb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ihydknvo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qghxcejz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omiyprdd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jlahkjqi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oqruuqkl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dyzmwpes.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3uoxrzrmu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3muiaixhr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iesgpyzi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdyccgph.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3riboouez.html


<!-- 参考信息 -->