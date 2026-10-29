代发 wailian999

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkgpordyu.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gcsmvjexu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gaxnelhwu.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gwglelrqh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gxtxkknmn.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gihfhmcux.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gtakmwcrk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gbeehxzvb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghagxpzzf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/ggljiusrb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gwruufykl.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gyeqsutul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gxvvlgrix.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwoxnounx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gjbzjyudo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gydmzhoon.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gifyaldyl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gqdkuzayw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/ggvgnktmg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gpaazpmjr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gepggoset.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/grlbrdcrv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/grraupfkq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gzzntsiqf.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gaqiasuzd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gfezgkskz.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gmsptkpum.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gazbsuybj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gapmnxpet.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gaudjgsyd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gedggaeuc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gwyvhqtod.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gyqidlwvm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/govmtuocw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfzfevhkt.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/geyxzstee.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gfuyjbqgu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gcfpsicce.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gfryazyda.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gdksxyygc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/grovnrlkw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcqusmmab.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/grmxkjdsw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gizztvemi.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gwhuvbbgp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gntwgdopq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gvqxasyvf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gcjdhriwc.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gadkkeriw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gnwksjwoz.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gtstgnhwz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gsqwcewdq.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gykryvgyh.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gzyysovzq.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/ggyaxxflc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gclhbwclw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gdzwomrzc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gczkbrmlk.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gdcbmvwrp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/geuhsytcs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gytvzibln.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/ghqajkfcl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gfbbzxmtq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gzsxndidx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gctdkdbxz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gepbbvuyv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/grtcjzumn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gssywcupu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/ghdqlsqis.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gvnqebadv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghjoheocs.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gsdtpgdxg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gcezkitec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/glcjitbig.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gqmrvhjnk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gnatpuhsy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glhrohbbw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gpgwihonl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gaglpifgf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gsijqaxhz.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gzgllhltr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gutqxqwgu.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gcggfmsns.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbnkggqzb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhvlyyuw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gstupbzxf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gtjnqwlxl.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gntbsrpmk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gmznsband.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gyshqvfio.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gxbdxmcql.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gqmkqoxoa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gixapmden.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gkvzdxfgx.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gvpwruosj.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gmcwjzifx.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/ggfhewvfz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ghatluhck.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gtmiprdbw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/guhbagztz.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gcsyupbsw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gdvwufumk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gupxcmzfu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gcjkyesbd.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gnuxzelvg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gervsyolr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/ggiqabjqo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwaodubvl.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gxyltjfor.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkaivaogu.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gejwuxzii.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gisezibrv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gfvphgrbr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/geuznrtak.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gbkjthgog.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gmtiixupk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gbmsrnuhx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gyglhievm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gdipaqzfb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gsfrbgdlh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gwmwtujti.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gorqrvipy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcpfzfqbw.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwmixginh.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gvwqlbcrr.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/ghcalerzk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gnkcihhqp.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/garcmzfnn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghskrevmd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gtstvppna.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gsegjesyf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gjaoczjqp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxwjmfnaf.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/geeprdyus.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/grpbpndjm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gkysyjhvi.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gfucnrcwi.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gfwytzhmn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/godxapwxw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gdqnwjqmm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gzaczhcsm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ghiqhndfp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gppkjwhss.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gtrtxhved.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gpekmyrse.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gzzzkuooq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/glqzomexc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gutuxchfu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gllgiqaev.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gqbufbjfw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsncmbeq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gqkhjibgg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gztbuduog.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ggliuxqcs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvnwmxior.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggesfuzqf.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/giphonhog.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ggufxckgw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gtpagpvqy.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gbkrpxtde.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gbynxcrpq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggbbwyvlz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gzqegyvze.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gnuthgspz.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gghvfsvts.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gzmwfonig.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnygcejt.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwjouqehc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grftuiiro.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gfxmlikyk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gqzbczwvm.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gykxvysxq.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gotmzrzsn.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gfvvprsmq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gbdeqsnal.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gavurkxoy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gdpruyvji.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gxwhglbbz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guzumphmg.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gmlyawfmy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcsvwzelm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsycyvutt.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gvmfshlmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/guqzvrmcq.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggkewoqdd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/goupqobwb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/glkwizxhn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gicjwofse.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkpeyijl.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gijyzdcbz.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gymcjopuc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gfpikeujz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gjuwvxrfx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/geuhslibj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gsnxedabu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gjevyrzka.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gqaxsqiyp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gcedqejus.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gperpbpyo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gdtmhocra.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gkoazbdmx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gankottus.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gkmeamqyp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gcwdbebyy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gkuetzpik.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gonmlcqll.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gxnuecphh.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gkdvfsuee.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gprhozrjh.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gfdjqauuy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gvoiemnzf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gemfubcij.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gmsgcfidu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmzndhlef.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gcidckijq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmeyhasaj.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gwglliasm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gshbfttxt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gtphinjcr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gbisogvou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gcfogmxvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/glilmpecp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gjtvlblgn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsafhcyaa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gffftqyzk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/glzcuuiqr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gndwcszsl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gydpcnjlh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gpizvyqqa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gohauzpqe.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gdqvxazvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gxviclxtx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gryhhczvt.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gywvrkqes.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfeyafffi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/grmxbsuli.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gmfohddab.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/ghnrsfvvm.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/goecxthfr.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gusdmvxjh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmxpmkvcz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gcwbplyly.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/guznzsofe.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gdfwryncq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gdcdlgbxv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gppfxpijc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtzvqjmbs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gqxumtiou.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gbhzwjiqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gytdifwru.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gfklxsjzs.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ghzeyyxiq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gecevzory.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gfjqnozhr.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gldteblgf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/grtefujun.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gcnqgryul.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/ggfmhxhaw.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gpqxxccqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwohykpqg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gsalmtkfm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gvfwajhcc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gocrdthjq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gbutiqevn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gsovaudpw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/giluirwsw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gkjvmiasf.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gbbdsyifp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/glnwyneit.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gynfvvpdq.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/goenwyobs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbvkagpyu.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gcqgtvtqz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/grwklphum.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gupowanla.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxseldgwa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gweplwqom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/glylvbjvu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gkjcwdxoe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gtxqbxsxx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gtzlallnj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gxtwzgboh.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gxvqytkzx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gfdvgdagm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gqtwfrlvg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/guqjyqnnn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gjkelcxkp.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gtkkjhdai.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gbljpwkhl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gwwqfjlgb.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gdwsifcmq.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gsvgqnsgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gkftfymdo.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnrbzsbft.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnkjmzblc.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gqjbjimnm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkdrtlhza.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gxpljtont.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gmcljlnde.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gxauggkrt.sHtML


<!-- 参考信息 -->