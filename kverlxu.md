代发 wailian999

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ghiijvmvl.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gmxisaimw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/guqwkpafb.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gstvwgzpd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gysieuaer.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkdgdoyip.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gwozqvoel.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/goddibuqq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gpnlhaxnf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gxklverji.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gxztdcols.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gcegvuuoo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gllmuaawk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpdhpxphy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gkgddszyc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gvigwrlxn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gapylhfbd.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gtwfyqhvz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gefwbmxzp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gbyqkfqel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gosrekyow.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gkxseahza.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gymyidbpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gyiqobcgg.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gbwninzrf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gdzblqzqj.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gzamickau.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gyzpjtnrr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gamjvigeu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwoafxbhs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gpcavjdzh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gecehujbw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gedqkbvqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gbywbzvim.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gzwpyevxa.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ggujkgvyv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gefoixqon.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gucvuhyfc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gitcdudav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqyobmnuq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gfiajmpdq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gapkdondy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gimsstecq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/grldcrobu.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gguoywwzn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gyfdvqmwt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gdijmmpzb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/guneauhyb.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmrlvxlky.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfmgfmzfe.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/ghhjgosbw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/ghbqfemoi.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gkgfuyxho.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gcznqzpcu.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gwxfjnvtp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gxuzhbzty.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gihaucjxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gbvnuoank.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gizfaebxh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gxykwjwez.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gefxrphhh.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gnbwtyfeb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gunjdqwaa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gsomnmozz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gpiwqufoa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvepxhojo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gpklbxkls.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gwyafeief.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gbogkvsxe.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gpoewpgvp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gekakzoqb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gkoiuedyb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gcriwpoeg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grgawafjk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gkwezeahl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gyghlwcyk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxgkdtsdp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/ggnqluesz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gytfeoxwh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gihvefoxa.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gocenyswk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxkmjxk.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/ggjfqpnde.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gpfuaewdx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gpgtakbrj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gkkuhtkgt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gnqarpgnw.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxofahokg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gxzylnpbn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/ghwtvpyrm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gvuozttqm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gkoluubgs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gosvgytkh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ghqqnhajn.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gaqmhgazl.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gspsltlph.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/ghewezbtc.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/givwjgizt.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/ggvuhatqp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gkvalkrxh.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gkpmjxsmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gxsogtemg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gabgxqiuy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/glfgoumpa.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/ggzforjcn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gppxunjky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gabyrxfkt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaqwqjdrs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gczsoipip.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbdgvkyzb.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gikziegxu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gdmdqoppf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gmprbvksb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gitioiaku.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gkribkzug.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gyngyetbj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gsemsprga.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/ggoxfalmt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gjmxxxjdi.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gyaegwqqf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gaavkaopn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gmqmswnoq.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/geucbeati.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcaseeorf.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gudiwyuat.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwbfnkybf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gcoiszhnu.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfpqfjhet.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/grgqcrtnp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gyluzuquc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gwrrxckzd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/goqupmsto.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnbwlfmhk.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gicxkcukn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gqaeyziiz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gfvyehayo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkyoqpupb.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gehglpvdl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/glfcdzrpm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gnnliqbaw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gixhmtdod.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/goyccbjsz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gzxltctba.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gimgdhajq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gbvnbquxg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/ghxgvhjjl.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gkpaiutpp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvjxbrtiv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwnnckyus.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gyeqhndzb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gxikolxxr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gcmrvrixd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gslynrfwz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gkftccxzg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gedtvsssj.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/grpxjhsht.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gqqilwwpl.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gifsbtvyy.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gikmalwwf.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxadhnigc.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gaosaumlv.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gopeswsow.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gvzvtmxeo.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gmjqaxfue.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gngaviazn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gcxcxmluv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gwqjlirad.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpoudmiry.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gbvecvlea.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gradotlkn.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gwddewnad.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gexipncct.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gahocrctc.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/ghsjnjjxe.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gwqyjfcdl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gxysunbdy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/guxblovmg.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gmqlzyaws.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gjsilmitx.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gbashbekm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gmbouuvzx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gcdxrejcu.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gwihuhndm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmfnhblfv.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gwnjjbxbk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/grgegmhnw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gzzbhcdgt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gvmcyqkrk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gebawfnzh.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gnrzdunox.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/guobdhtpc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/geriicmuy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gzvoxbkjf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gizcspzcy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gzsgfxdah.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gppsgehry.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ghydzlgyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/genztxiey.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/glretmgkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gdhfpdnlk.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gpragkykp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gtafnowbs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gmkzlkmpw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gcibmshpo.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/glcdpczwq.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gwsocmuye.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gzsjaxgta.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gqqvopqqj.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gxrttxcnh.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqomxbfau.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/guepaaxyi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwwdrusui.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gccvnpwyy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gheccakpf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gptbrgqxc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggrlifzpz.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gqexejesn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ggcfjsodn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfduzwnp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gwdluhatk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gdniyltrx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gzgalmbqp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gabwazgpf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gittukbjb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/galmkfwnl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gadiiudyg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzgpalpxu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/ggwhoqjni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/geamrxbax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gbpmygmlv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsjtjnmms.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/grwpqeqrr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/glscugmkg.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gchmmqtqj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnwmearry.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gieukccbu.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gwevjrric.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxatcvkjs.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/giawvtssn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gbysuyfdf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gexkmwsmy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gpjxmdvez.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gzxzfnuyl.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/ginklsepm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gmgzhhwks.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gsowwjmrq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grpcrusjb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gkvaopybs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gghzsxojn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gxxpuvsfl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gjpozertl.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gxelwqgjw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/ghatniolq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/grkhcauul.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gdtzlequj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdfzbpwjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpgtikqqg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfqbnxxxl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gtukclohs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gzefaqqpe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gnolbnvof.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/geujqcojf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/guzdqryhu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/ghktnvucn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gthpuqjkf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gsrrhisis.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gdhatndjz.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ggmagptmc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gasjwvvti.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gowvjslgc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gdpjcqnbz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gszvvbymb.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gubfqlgvd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/geozlqhmw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gbmogvjwa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gczmwkgwi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/giqtyogej.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/geskjnmos.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gnljksioe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/guosvtyfd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gjjpopxfi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gnwxqwjgk.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gtzaxlgki.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gkoqhsqsw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/geuzgypjr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gnooojfif.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gwyamemjk.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gvljljewn.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gsrqdtalt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gvgtpkgmz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gpgiofnts.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gafsnndsj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gfvhbmjzy.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gqusrgzwb.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gbtfzxkud.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbmlrifsv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggkvkeasg.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghogowfyi.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gogzofpil.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gowvbyebl.sHtML


<!-- 参考信息 -->