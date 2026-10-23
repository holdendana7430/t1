代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bfvwwufo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3irkhmlvn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dnrdhtsr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oivmzpjk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3omtrbjcm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bemxopgq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jkbrtgfv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3usogroia.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tyakfkue.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gyeqkpcs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3iiwvnhtl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cjjoiyky.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yaixvbuz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vhmwtehy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ojqtqauu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pqlwmrfq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jjkxqjxt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mresantx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kujczerw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ipscgbxw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lhjmzecl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3snbrefiq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yftwqhqx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rxhybbjy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3orfsycgu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3evitgpir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sjskmqmz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wqnivqgo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nntxdpto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vyzqafji.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lypetcri.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jdjgmnit.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ykormkvn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzfesudl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgzsnx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rdpomwjz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wvnnmeyb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uzcnauvd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lgxqcftb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3litxzxzr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ilgepwlr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lahprbyl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3clntdzmz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jaevbwdg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3biieujaf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zsujhtul.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cyocbkwn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dflspxro.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nachkzoq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nnphblzp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cestlrhv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jqqgufij.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gcmydbyy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3asaaaobm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3eenalkac.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hmhvqkle.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ygqnyvmz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mblzkowg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zcjsyzzu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3olmiaxgj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wgrcsrfb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tlzcxloy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3twvxnxhc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xfxxlxre.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ujrpubcw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3egsqjhph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ppkcwjnx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gcblazox.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3etylmqzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqcdwxhj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tycphjfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efekjjuw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vvjbnhaa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ihivjrpf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bxgrlqtc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xmahiskc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qalxnlbj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3chdjjzbt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xchjvtii.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wytdyglq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvrwzqck.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3akcsvabh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ndhyggjt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nshpzoek.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mlgajqix.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wzmxgqen.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3duchfhce.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tuwbfdgg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxyhynsx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3movolrqj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cdncvzgk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ojggdgjb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3brckzfhi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3inqwssrj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3quldskzo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mwlqcyey.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3chdculyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tdjdszmk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vxnlozat.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hjrihqct.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3scxkbmug.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3usjvdnac.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3iblbqunv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmeqllzx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ogznjipd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quggsboo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kxcefsbm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mqlitbag.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rnkduhae.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xqcrnqig.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jilqcenh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iqqqpidv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kvdcpymo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3otmugcxy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uxphczol.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3falfjumw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3voownafr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pditlufe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uxbpmfqb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fhjdukcr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wuervyjw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dbktnjpa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3chjgsrbo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kfwuatpt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dgqrvqhf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uncfotaz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3prwfouoj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3czzlcwjy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cchtnksc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nbltqpvm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xucryaua.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fhvprbfg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjtzbsu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sjzukwii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ruyfobvd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hgbvlesk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zsudczvp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yuwrzdmr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ioqxxoel.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qypzxwws.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnfejrd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrgupexo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ctbdchzw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cgitdkov.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3acnzuvum.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dawjgtpt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yakjlfyo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kqtaaxis.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fqzpghve.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pzshpsho.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dqcbjkbj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jbglfvte.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cylqmjpw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phjaxyip.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kstqylfo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3snyibyib.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vlcpzqoi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3trxcpdan.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yhewmqcz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eoomqrwv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wndpqpvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3simzxwcz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ozntcdgj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ndddeclz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gsoupujf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hplxksxr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ajinddpz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bryvnfck.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yxmjjolp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3euuocwex.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmybynyi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ryxojbwt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3opqxdtpf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gotykdmv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ynfotpyg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nmzbdzkg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qkowkgqf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zbvslfax.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wxlsgiem.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wzidfnmj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqqwioen.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fuxdwvkl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cbykfsbo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fguputme.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfzlymdj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3exvlugos.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dswnynww.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3phlwhcon.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ltfzawnp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbmnckwj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zdrufrtg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uivvqsyl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sofmihmn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kqsqlwoe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvfvzyqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cctwfyrr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3evqrxhvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sbzegqrp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjyknbdo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jvqprhnc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mzxgzgfp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jciixlvz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgfefip.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sapmqose.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jyrpomdg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pszggwbb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hdrseceq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vwzfzljw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dufouike.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmbzaik.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xypjxpmt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3krvwjgbm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lizolsfz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ffigzpyn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ocdmhszv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vwqkldtq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xvqqxvbq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3szzmzygo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qnxlzvob.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eruouwxn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3omziehyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lopynpzv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtjkdntw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ubchykgv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3skoqlwep.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tsnruhku.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqeakyt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emsidwno.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmrhvxvw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnwugiqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vluvoatw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrqoegai.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tqgogmwz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bvsxgepk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgvzpres.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjcoirlh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ycxmbzzc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3snxntdvl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uwhowkwo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xbnqfmuu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmyvnpjc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qelzkzoc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uffbqkeq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3smnkhhfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gifamqgc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lqikpdzm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lkvqyufx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ckkcljfq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mftkraae.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kpjhymlv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uutxqnok.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzeuyyup.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3njrtgkva.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jaaasqtk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sbicyvzk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbbcqou.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsogouop.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3soldxdkh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3epovgldz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rqdgidkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fbdpmuln.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mpjznwqh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rcbqbakc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hgsqsipo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukdsazau.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iuubanjl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kcuychjl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ddbdetxa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hkiujypq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxrqvcon.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gpueaudi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hwiqzhyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bwjksdhu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3clbcwudv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zoknibvk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3doroasjf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3paiovuuk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rxhinrtl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqydslam.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyhdwluy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bscsklwb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hpjafzwv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3inwfcfwn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qzeazxzp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3veybqsgp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cbwcihkd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ttbxmthr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qlrqmnop.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkuaiwmg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yctzrilp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fiodlgbb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivegnafi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3smnsziho.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkazjlcg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cndpngfb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nvjabixb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqaztnx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3snqhedtz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyrawlz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zopqybin.html


<!-- 参考信息 -->