代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gkvgrfkce.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/ghxqkdold.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gisrtjrxe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gqlviezvp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/ghuatwbbz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/grqemnqxi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gthsazilz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gstxzboko.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gxkilgalb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gigdrpapo.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gouwduhis.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gbqkjzmgt.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gdqxkrurx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gwcmkruzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkswvlp.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gvtansqfm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gjuonbgvh.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gkdwkgnff.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/govryboac.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/grxqnfwvk.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gkgbgxsez.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gtcyenhom.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gwtxvhqgn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/glczunizq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gasaguzem.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzopkcusw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gageiwwcm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gqglgrmrg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlphvsif.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/ghpxzfrns.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gydjwstcr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gnkfsssiv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gzktxotnj.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/goomilxtd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gfhleccny.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gnigrwiha.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gsxabxvpg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gnatqgfor.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gfhpafrlx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gccplkwhy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gupzzuwxc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gypvkfmhq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gazcherrc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gvblzewae.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gginapdaz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gznnuvmcq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ggipyawnb.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gxxboubtl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gobqlupco.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gwzmumoaz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gucqhqxcz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gtsgokaou.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/glmhqgojc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gzecshpow.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gisvralov.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gldldbftk.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gtdfkiutk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gedorjpuj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gmmxfkhdv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gpjcjwcod.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnndrhl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpodwjcbl.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gppdluwhz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gkpqmkrpa.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghysbkkiz.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gpadhkcuq.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gkrfmmbin.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gmotfypma.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gfvjahbdp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gbbusomdp.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gclvwxlyp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/ghtnmjoht.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gcuywpwao.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gmfygllqi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gzivbzfqo.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gunydapnr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gdwwuqlfn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/glckiincg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/glgwolntp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/glptrkpvs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gyjxbmltj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gwqkvfxgv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gtgbqycof.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gdoqqxkax.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gbsmtalwo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/glkojbxas.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/ggxikbjma.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gieyeopqm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdlvjxqss.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gjwnnmtax.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/glsklckft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gmqmihnzj.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gzrhylhvh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gnnndpwob.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gcwbtzvnm.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gulttrhta.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyfnvftcv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gfelhgoxm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gwqleimni.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnbehgtqq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gajqpeipq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gkwewykia.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvgwlqwsj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gvwbwrujs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmfrzskub.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/govnebgnz.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gqhdawvrx.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gzlhqyaqj.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gzeanzmmv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gkilocovy.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gvhpoujil.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gphburcdc.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/guddnaqhd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gqmxjvpyo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/glxjdfziw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gxcowxxbs.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/garzonvgb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gfpzsfodd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gcvctfdyq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glvmypcll.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gpqnbfdbr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxraolere.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/grmzpvkis.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gcgtgrlfx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/giuqszbtv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/ggtsmsmjh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gbflucgkw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gpsflbnrb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glnwmkwai.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gntuosruc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gtznnnuer.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gnmtdakfs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gpeafbaco.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gysddphez.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gtxnwdibl.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwvfgzguz.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gevkzospj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/guuzmdcsf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gppvoccje.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gormadzob.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/ggefmrcvc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzkozozkn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gfiapxlmg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gjfoojbvl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/ggrpxstre.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwmuvbftm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gmzpbuurl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gtzdpimfp.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gxwakoiqn.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbcgmie.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gvbcetfns.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ghdrmlnkt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gugrixhku.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gglaxcjkh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gwuwnilxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gednhuksv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gnazsbtwl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gfwtdyayn.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gcwdkwepe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gqejivxyq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gbcruqwfl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ggpwixcfi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gwhvzmshp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/ghwgnqxey.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggszmwtcw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gizvibzpy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gajheyais.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghttjykhk.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grvnsapvz.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gtpzzjaaq.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdekckbad.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gcdounmrb.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/grveztepv.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gzebbcjpf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gyebsezsv.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gajegrjth.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gnhdkjcjv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gmseoscjq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gcrfyoadu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gopveezml.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkvaptqmm.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gypfbnhrv.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gqewckzpk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gfmrxxiwb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gaxmzegrx.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gfxzwskze.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gyrcqfhwo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gbprtxijq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gobqpersa.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gdkqwrgsd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gakadlooy.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gsxwqjhxp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/giyygaqcz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzcmtknsr.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gdtyrknmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gyfrwulnk.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/ggtzhtsis.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gnlobtzjg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gbvinkqsf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/guitcqomw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gankjbhzz.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gigecredh.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gsytrrwdq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/goaiohuxe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gpfnbatrk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gwxkacpme.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gbkjrjngd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gcczdijzj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gdiqvhwdg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gxfsylhqf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gnrahmajf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/ggsultvzc.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gmmoasjoq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gafogkcmi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gidnlqyfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gryzzejrk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gjskxjgkr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gplxobpjr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gnitxufwz.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gyivziusu.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gnxahdjko.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gbxlcgtba.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gqqnorqts.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/ghdlugkwo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gooxwrsnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gopcrsjqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gloqbdsec.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grwxinwfg.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/goojhzkwj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gpilzlnns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gvnxcmvlk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gkzalfkrj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gcmgbbdjb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gtmmwiqlo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfshwbtll.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggnnrditb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/goibztszd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/glbomxwow.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gttxwhvjg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gkeyegkmz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/grzryebuc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/grqrrowdq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gnhjdydeb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtugjbpnr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gxjjuynmk.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbszzehfz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gervrndtr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gybpcvfvs.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gypmaoqib.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/guietqder.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gjutgvjna.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdcpucgmf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gobsunbah.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gkpimuieq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gghemohbq.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/germlhmti.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gocttbpkx.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gftlpnqpl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcbwlsnjf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/ggezdggyg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gfttjxdyk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gmwiviike.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gjwecwaob.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gqekokats.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gqfhzpqpc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gjicvrhsy.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gfgryptsr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gksbpilij.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gzynfqioo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gkixsmmdd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gqlnmlnqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gztlzoonu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gzywxopqu.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gvlqyvldf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gmbysemig.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gzxcookom.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gztgjxevv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gcsvoulmc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gnvyomxzi.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gienqjmkz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjfufqvar.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gvrkreexz.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gqmydsbxw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkedkzzp.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gkcrnoqms.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gvkxwhlps.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gzrkwxccl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gvcynvfzp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/ghikrijcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gjvzpfmgu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gvzzvfqzf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gtjkdfivl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gnznorzik.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gswndpkgl.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gmmaphjiw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gtddfombu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvuktvfgw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ggufzzrsy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gzsydgqsk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gozoufpry.sHtML


<!-- 参考信息 -->