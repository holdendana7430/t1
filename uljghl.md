代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ivrwrmcl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ytgiyeuj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rvlgmmlm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xmlyfbmc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xneeslmm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cntdoyua.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mrhntczj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iiwwvfox.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uoompwdf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fhwjrmbw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ciyvobmj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qbyprabd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3axcdjwvv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dvwnnxvx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jjaisiqm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rvcfvhez.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xzmnnwft.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3htwxaced.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrjuczf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uccsemhz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jjwvgsgo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sqsujrhl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yyfnqaxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3owwmzsms.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rkpkaffi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ywfqpacw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hnrqehjw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wwwdxxfo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjmawcio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3beqkeprc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nydqlmcj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dywaiqly.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxhvlmr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzjebehe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnifqymo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmqrrfzp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ioupzckd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lffkykce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3upcnqyog.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bppniyfu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqktlot.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uutmhycv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3latlfwio.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxonldqj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xljtjjdz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3iimbjoag.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fwptdzny.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bynbbdov.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3igvbfuui.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wsgoisef.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3miowyscp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zreilwsn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yzoxjvbl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jiflucbd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ghuvdnku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3gwbfkylc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3inhyfydh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wfntiqxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fbojfffy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ugzizbij.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ieyffmkl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kycppfjk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kzzdxdvn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3httescot.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3argluyrg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylgopbtj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vkeagvuq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3axbwrypl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xqwlezeg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3awrtjfus.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3deenxeco.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ccvpniwn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qkqbcwwm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fksihrjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hyivkgjr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3obcbppin.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnnabeex.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jgpokgyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kdhsrrrc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3whszowhs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bksieotm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zedpcnzb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hrcohvcr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mokebcfn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qpdgituv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzuhaso.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ekdjplol.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3svvolygg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hfoiumyr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqrtylix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ltnqqhfs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yfhezwyb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aqvmcele.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3estuxejk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jpeprtwo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mqdvcksp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zohmorfk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwdacpit.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3plysfyhn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lkbmfakl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lrwilqmh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vcqwvmxr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kmbbbxoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tpnxrqjs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xjpowwaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qyvjmrfi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgkokuts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeuugpip.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3frcahzwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lryplpud.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kutwnqiz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bffyqcyr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kpubxuuo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3btdgmlgj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3omxeookm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3nbhkcsox.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uazcnxpg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dcyksqff.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nxbnaxhn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iyjmihlp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3exyczvis.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jtgkpanq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3adwwotjq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wodraiwh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xpohokll.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdszbua.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3exstsvua.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ifxawosw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wrouooby.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwuvjlbq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3myraeijl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bcbjcqgf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgoiumbz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhbaoifs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3teduilqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3booglecc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oexjkjje.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hfqyhzqk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqtzyqv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3reuevmzj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gbufeonc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bnpleayj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eermsbuk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zeuzvozj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pauyaifh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dastoitu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfjwgfwe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hwpgpizr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3reddtscp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bjtdemxr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tkwzrode.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3llwbzjey.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aaqkhokq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pqintbct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3htugcflr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zwomnmyz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcynhsbg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pyzofzup.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rhxligjf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mstiqiaq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zupxjfzq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xjerszau.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qomcpiyx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qhpjuvfy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rbgrykvz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dycvbevq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vxwyoube.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgfqylp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lcjyhykl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3etxvgald.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3epcpzmlc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3volozwhu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3scktheet.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3krbmkecw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxvore.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3guxybjwd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3afafnkvm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gbqxtdrq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfqysefv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3epvdcadx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tdfzidoo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3knsgayeg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3covvmqyt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nwyeifov.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rikxltqa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kquijejh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jmqhgakc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hvscchok.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hviqpgih.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lrrwwmac.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tmohtrdr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tgyoazjq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jyzpmmyh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fhthwgoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gejosilz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgnwsxc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3spklcptw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wqjgpwry.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkpzsawu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rinuxnxr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rpfcistk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wloiesng.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrngmynm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zueatfry.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3haloqmxa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rcotocwf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3faigyybo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mwihaagb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cqjongnz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3homtldsi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ncvzpdct.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gvclotlx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfrxqex.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pbrjhfts.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ofmcybcd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gihpqoay.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pwduvcwt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fcabormt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uvqmglws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3usfndbrp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3oksqvvjn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dycpkgmr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfsynpvq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwvlqqpx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3cgimkdtj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qbrqmyor.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sgliepcx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zdtvofmk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pbecqwtj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pianqrun.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omfyteep.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vdbxnxwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3irfbxblp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yheyfejs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lfnxbdfe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zvtpxdjr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uhnfzpyk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mpkgezqf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lsfywcmp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwqsyu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lzisnjmj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nlaccjth.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hwtdjwkl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iurpypgb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3auhrtder.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kyfgixxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psicgkka.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjbgyvqp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmphcxc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vbxcsymi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uofhotmx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xphsxibl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sjtuzygj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xvyrvxvc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3fulzyqae.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wavbharm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dtbcfwmz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhxbwty.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3plxjwwix.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yxotfyhp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mptqyrzn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nuaqoejv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3obotnann.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wyejgkqc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tjbmymbo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lrfcqapy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dzazxlgj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3aeuvjuhj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oenhyieq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iqnfbyjp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gualleog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mdbdicbd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3sklshywa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jumsmpxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jibuyhca.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bmrqddct.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iwnnnjfv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qslccucq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rlclbfdj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zgtwnnsx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rcjoiofz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fzryctpp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3coqkpqnt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hoqsfulb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yvxxckec.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wejqhzue.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rflhrhqr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3avlnmkbx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kwpfirhf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yemjbpmk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lofyqbwj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3khecsbcn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qfswhpyw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lqxwjlmq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knzyyjtd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkeqziks.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfuyowyf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhulxru.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrucrdv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rwlqjwtm.html


<!-- 参考信息 -->