代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gyshwnjtd.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ggyhexxvv.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/glwbnooey.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gdvftmscr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gocpdfbkn.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/grzgurqjd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gyqhefjur.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gqrqmhuqd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gumyvkujq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gjvafdapw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gpzdwljqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/giolkrprv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/goqoenmpv.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/givzquaqr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/ghqvprgij.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gbzfdpeqd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlptvrst.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gitohcjko.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gfhusvtoc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/ggtbatkgj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gwmxeppep.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gnsjadter.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gwnyrqffg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gykdtojik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gdgfnsomx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfvtkakbf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gwymscgbn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gxbrqreke.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gosaqsena.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gspljljox.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gsiqlcswb.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gqhezhjwd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjtycbqrl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gjbtcctyj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/goenwtbav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/geyxpwfnk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gbplersoj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/ggamdzswd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ghheovqre.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gnskbpmtg.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gkgekskkb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/grcnwndnh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/giyqcyypj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gectnyqrg.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjipmwhoe.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gequcsyjc.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gprekokfp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/grfgbkuku.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gckhofwdn.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gwhiokdkb.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/ghdzeygsp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gbvzdhxsm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/glzkcvtom.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gezteyjxs.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/grhpannkx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gyhpyxdck.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gtrkakhzq.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gffxzerjd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gomnpwgeh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/glybncugu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gcjneyzwk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gcfujtszq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gbzdtxwwe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gtksfdfsy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwlojirfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gtzrryztr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gkxvluzgn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gzgxopkug.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gtutpbuor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzzmopbzs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/guiwxbuvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmagxkefx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gbeqbuwxa.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gdsiwewff.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gqwzxskqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gevtukogt.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/guevgyrry.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/grjeuqhsh.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gujuuyauq.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gztyhtnji.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gsqyeqomu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gyckhtqms.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gsmjngmqu.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/guspzkyhp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gxejgowmt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gsawvolul.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpmdbak.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gvpbonjzg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gxtlezrxe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gnrpbhnqc.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gukxayzpj.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gfanwccpn.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gemsflmla.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gvghrzwud.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gaxtztrki.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gsahnrngq.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gaipwqxbq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/grleqatow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gtdwbdlsa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/goojyrahw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gopjhwlab.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/geupycugt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gcmqrzwuu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbthyaszf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/giyepusuu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzjhjypwb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gyjxvdyyl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/ggrrqjtgg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gixcizoht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gqjvtchhj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gmlyophvl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gdwrwteck.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/ghnqgzohi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gwxaorofn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gwtxewcib.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gnpabxnaf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/goyuzenak.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gurciacyq.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ggyszyvvp.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gworkdjxm.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpogcheav.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gzemxbnnm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gftcbegqs.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gyphiutxp.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gxdfjlbld.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gorlzlywi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gzpwxpdje.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gyflwhqba.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/ghkcsjgwc.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmpvfdyed.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gadqkdkwz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gsbzjxiqh.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkkdeevkp.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gvgwfutww.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gridqmfqg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxqetille.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gqiimliok.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/guzmkrftc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gdgvyidjd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gmxnmycvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsqhlki.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gzizmwoqc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gboyufphf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gsfcbpkdg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gxroalfae.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gyoixfjhf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gbbcindug.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gzxcpmbuf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gzatdjbfo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gbbwxjaev.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gskxcnprd.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjsrougvo.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxzcdqzck.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghlyaizot.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gtuhzcvas.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gqrxpywsu.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gsroeycck.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gmotzvvbj.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gvquqjsxa.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/ggcqqvxub.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gxhwwfdgj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gamaodtvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gugmpgwog.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gazfignho.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gisromwkx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gofvehawm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gjisbryhu.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gaoccwyoj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gpinhjoqc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gophdagou.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gclqsrtsf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gagglhxzk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqjyavpnp.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gqwnmpqsa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfakluutb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/glchvtkcg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/groubjrhq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gwhdnfqjh.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gdhqvyntc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gtkpztgqu.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gakydjkft.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gajhovpby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/ggiaaaodr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gocahtqml.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gcpdlcaax.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gcplnnwyl.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gcfxvnarp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gpwasehfn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gkihzoefl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gydkeazjb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gtsoieoec.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gubsajiaq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gfglkznwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gfnyqopli.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gswuthaaf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gxcldoljn.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/grsxzhwar.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhtttfw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gsbeywxdt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gpfhujgan.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/ghdaudbut.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/guvwqwgog.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gsbftskvb.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ghxtpnvgv.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gsovlhlxm.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gdadlboud.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gnacqmrji.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gyfufmmkq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gqljdehlo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfkodohsf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gvqitlvlo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjgofwdtg.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gvvyeedtn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gygrgujzo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/ggqihydcm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/ggbhbxfbi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gfucvsnuh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqqaqnepq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gelfthxyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gvbrkzdhi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gblbhvdwm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gemfalqei.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/guknsczye.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gbnjxpjyg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gitihzkzb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdldupvwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gfbwafquu.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gpdxwjgsc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gesrbofcl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grcctxvhl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gkhhkqckq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfamodort.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gqqgfdyqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxbyshpcp.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gjhtygsng.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gcgzgmgmr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcbwfesfs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/grrubkkqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gletkijtc.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gzlmclhlw.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/grqxcpfwc.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gikmscqgn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbvilflrf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbmywnutm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gztzdcrvl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/grjzdxhhk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gzmsuqeop.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gtoecqqcd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gbujntbuy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gcdzhspcu.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gtxrqytvc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggolexmnr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gbtzxbyxl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gnstswdyq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gkxhrjobd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gaejvvqbs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjabxcvfq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gojcxwhlu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gnkhfgugf.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/goazjvxfz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gzwmgesgl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gbnoofigw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/grwpnimrt.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/galgyycdg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ghqzzvvmj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gfxezgnoo.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gkgndlimr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghiakffxp.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gyqhmayzv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gjpaggsto.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gmnwljnwl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gjgxjbqzz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gidtopsnz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gpsnpyess.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gbsphxsyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gvrxqxvvq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gexazhimx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gqgrncadd.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gujkqctso.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gjzwzfkap.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ggmvoamdg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gsjlulbjf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gimjsxnxd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gvtbesudw.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/ghasrbrdt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gvqujpvlq.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqidkufyo.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/ggocbqknt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gsibqnlwz.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gjcagjrql.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gjbyduhfg.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqaxneuah.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwnfhztgt.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gmamellga.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gmxfhqdwv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gmhjrcvwl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gycvvnecg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gljrfdmvm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gneplybgs.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gfkzzlyqh.sHtML


<!-- 参考信息 -->