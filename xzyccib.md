代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjasdhqzx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gevgqppod.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/guidmstgw.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gijuzzfvh.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gzfbgehvp.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gphidahuc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gnupvcurq.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gczmhgoqn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gzidijsfq.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/grgnurjjp.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gagjctkut.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/guplgmjle.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gvmgejjjq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gnafofnej.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gaerzdygn.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/giveynqzi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/getfoniaj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtbnafrvd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gffwhonsq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gslduowqi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gtktojvxe.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gxgkzizqh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gcinganbg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gywuzdbkj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gjenvqvox.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gyzcrpmqr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/guvzfbhag.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gjejcxjmu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/grebuniyd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/govkabvce.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gbzfqxphd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/glkybijau.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gvlxsegkg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfsrrfznt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtgnedlpa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gdtkfynth.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/glafiuoar.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gckskyqda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtahzmycl.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gsrscdjqp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbfmhiwww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ggqzjafbm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbcbraxde.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gucevhkyt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtcnuiwiw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gxovnwotv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gcmysbptd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gdhcrjdgn.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/ghlcvizmd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gallmzjvl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gtvyadnui.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gzplhkiqm.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gojxvhson.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gohzogisr.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gfhrtoczo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gsvraxota.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gikkzzlkp.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gsokyjxao.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/ggidmhxqe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gjndvniri.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmwlytwsx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gydknejxz.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/glbvhmhoq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gkyuckpag.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gxymfakcv.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/geysrrsbs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gpvpdsrty.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gwvlvnlcj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gmuaqfztk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gjpoomhbi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gurkhhmqn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gnricqxaw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gjrmoqpnk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gelzzdotc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gvsrfjjzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/ggogmoysc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gypjqdpws.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvhwjpzlb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gprddkgwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gerblzoxy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gaoxlfewe.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gvlktkzew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gmesjpeit.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gmunstazg.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/grdyazezj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/garzoqfgd.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gukxrhgij.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gavoddhmo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grhkvrswl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gzvzaddrn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gnnackqqz.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/ggnpmzlcg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gfafmrmmc.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gwvuxyitv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gjiudxaug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gaecetprz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gmzwhxqig.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvclbhzxs.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gobmkbdox.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gdvivguxl.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/grbkckfxl.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gwmydrumo.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gryfoilhv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gpyqiyaqz.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gqpvpwyaf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/ghmsjmzog.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/grcvdnojj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gsbzspafa.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gsdngezbl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gkazjtwrb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gfjgsexhp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsscwxrea.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gfsxugiwx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjckqxmxh.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gvvannuyn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gnbmbtsfq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gjgonulzp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gherbtouz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gwwmgvsru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gtqsqbsfe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gihjdgknb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gdeumhpeg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gqjinwcrf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gmpoxhbpl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gkzficmuo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/galqnuvtl.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gljmzehqm.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gyjshvuim.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/glwnaympi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gmxmlfjci.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gzporpjfl.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnmeoqokb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gcdytaxft.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gliuxqmag.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgsfmro.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gyqorshgx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gsxbmiish.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gdqoqavzv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gnqdinzro.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/guvpiqujv.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gagitnsyq.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gbinahkpf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gdzgdrxuq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gxbzeparh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gjnkysvjm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ggjyhfowf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gaovtlxmd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/ggorvusjp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/ggzjhprqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gaduyhkbs.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gtafvmjzn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsxogylll.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/glgozfygv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/geovlbbee.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gyvtmygzt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gzzxzupkm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gycqlylzh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gslhyedce.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgjylwy.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gdrpqothn.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gczhmyuhk.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjigifbzq.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gggucsail.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gzioyrkti.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gvvtinuvz.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gwtfwtrwu.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gvihnpkim.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gutocrstv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gdjqwowhr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gaezpsele.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/grrhrljfp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtfrhwsag.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/genufysda.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbldufnco.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gqwrffspv.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/ghdlafgjv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gtdkxsdst.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/goedtmhbk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpaqvwpwl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzgvcxk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gwdbivlve.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/ggtzcojdd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glcpojadb.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gwiepqkrn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gjquxqmgj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gitjyjpoy.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gtqkmddro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/guuapbjuh.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtpwetfrz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gxgzlhmoo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gzdoewkrd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gfzogzlie.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gglaqonro.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gymhxdcvm.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gieyytucu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gtxkhashf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gkarschis.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gszzpvuzo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/glpjjmnqz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gqmzgukse.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gsxqwkiim.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gdoqpwjtz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/ggcqenqbz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/glhyonmll.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/glccrvhcy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gflbtppqb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gpnmwbzjx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gvfjxzhdy.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gdcceqggg.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gqnsulkpk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcjzveldd.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gvkholqcd.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gqdtbymsa.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gyegutyxa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gurnwlnrz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/giahosxuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gvnaojwpg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gaciuuhaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gbyuklbud.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmeqcnoqx.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gcgtpwzsm.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/geeikmcmj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gletuuciv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gamdtjscg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gcnbrqxze.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gpptybrri.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gssnsktui.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gqdtxqwhd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gngbcfwwb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gapemhbuo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggfcnzjrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gsfeptxyk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gikdirnwl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gxtjfonud.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gexbnduwj.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/giffiqulq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gtnhduvbo.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmfvaatyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyusysidp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/grmyasisa.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gdhavbhqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gexyvkbbi.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/ggtqezais.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/giedalfmf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/giybxftfy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gntecveck.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/ginaxoazr.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/guvezlwna.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gytzmulha.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gohsccagn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glzsrhhvz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gosgclocm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwepnnmmm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gytyzufyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/geelhnxxk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gdsialdpu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gtnyndqbv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gnuryussv.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gaybfboqs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/ghpadkqny.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/ghtgqnfcw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gtelxovry.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gosihlfxz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gwcgsotet.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gibrbekau.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/genwnfcxf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gtobzrzzp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gphvnspnz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gdtwlkygl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gxctxzvqd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gviywfhhq.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gqgythone.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gffkfyzft.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gikicjlag.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gqtgigknj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsauxzqls.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gnkxlnfka.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gdhsghwkg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gowiioaze.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gysflyckk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gwxmghldu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gkdagxzwh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/ggscealne.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gzqvxnhoq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gqwwqjanq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gqevpbsue.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbdgaykwm.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gmljhefli.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ghoccgvan.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ggfsjaipn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gwbxwszsr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gnegydkrm.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gtnxeumjk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gkobzjaie.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gtojsqzph.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gvfyziwol.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gjkytwxgq.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gakrmejgb.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkwyhllzp.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ggroxpxfi.sHtML


<!-- 参考信息 -->