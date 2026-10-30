代发 wailian999

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gspwettgx.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gxbmenvzw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gqciwgtos.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/goadmvbbd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gilpydvgo.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/ghksriayn.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gjgezvjrg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/ghkxtagke.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/guueexija.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/grgaxvksw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gthpikrfu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gmssmfmeh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gymzwsnms.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwkjxorwj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/ghambwlit.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gorwehfbj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwqgpikcx.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gmkqviwtb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/ghmakoqoq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/glnifgggq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/giwkupjcl.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gqwxvxjlz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gxknslepr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gmxxvrtcc.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gcthfldbo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gwhtacqoi.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gffoqiryk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gwsttamnj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/guoptqefw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gnwfdtkvn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvimkpfug.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gmetksqvq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gfqkimclb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/grtpymnex.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gkahlihdv.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gfceaeftc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/grnjxvomv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gnsprtqah.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/guleavhwz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gaqmdxcyr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gnezvrxih.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqzzdku.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/grcqcfxnt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gyxycwkdw.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdpgoqqzr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/goztnppuy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gcnrsqqmp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvkfvlldf.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gjoccpxpm.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gllrczldl.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gtdzgyyvd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gozmrrycc.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfpwwmqat.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gjdlydhjm.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gdskepqds.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/goqtidzjg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/ggfdfzvbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/giinucwwb.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gzzomhcqr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gpvsxrvkx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/grhlrvaet.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gswrfmwnw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/grphbirff.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gkfhzdqto.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gmpuypkxf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gftfjifaw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gwbvmbnnm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gdezftooc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gbqbilptx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/ghednykkc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gmribjbew.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/ghhfrustu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gdglmneyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkrlzpqbs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gvbnqdwbt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gegjlgtld.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gzjxjwcaa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gfdljloam.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gklxdrfwp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/ggktvndlt.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gfndfzqcm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gegegyfbj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjrcqmqur.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ghmxroida.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gnyyhsuht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gbjijoaad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gwgsrnjhk.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gztpzrdrs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gdniiyryo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/giwilpmyl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/glhkelwdh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gcmzqxali.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gxvdizdks.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/grkjxzfbr.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdieamslm.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gxukghdvn.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/guzyoopsi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gxvjefuad.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gmzbkctqe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gmxrfvfaa.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gpkbvaioy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gcqsiryax.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gioktlckf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gphauisre.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gaqoqjqxv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gfnqqqguk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gennfjqdp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdokplbnv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gdrbkccbb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqlnpyckz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gcputewkx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gqpbstqwc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxzhwezbj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqqadfofr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gsxptvxme.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gsbaxzwms.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/giapiokxm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gppjenmgf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gssbbmzzg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gfbfkfpgm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gismmwhkf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gdczovvfk.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsaowyxut.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsmlgvgfz.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gbnautunl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gacearusl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gwuohexyn.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gfbftacby.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gkmsvukxr.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gesczitmm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gddkfcwdk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gwsnzrrrt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/giensqdhf.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gctkmvuma.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gturlvhev.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gvrurjeib.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmyckwxw.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gjxulndud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gncfjtzae.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/grgslqwix.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gzaxqebdu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/guixpxcvk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gcffgalbk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gboioczhg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gpovcpkyy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ghmevckbl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gsyhhyhtc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gewbyoiwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdpzajimh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggclmoryf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gatwsdwul.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gusxaatks.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gwbnfmdsm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gfbkxborv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gjiuzeeih.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/goercylnk.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gnduoqaum.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gxlfdgklz.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtnbhzphf.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gpmyzahhl.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gobaqbszz.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glcywrfci.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gcqgsuuxf.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/godesyblt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gognltluw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzipbuo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkvlbfxpe.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/goreeaqdn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gtgxtwegf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gnirhmilb.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gwknpmrvk.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/glubnmqfo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gnhuaijqv.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gyungouix.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gssaaqcmw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gzssvkkgp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gbtcdwwpe.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gzsuazgpr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gyhtagxef.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gkopybjxa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gpgqdelar.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gvudvkuov.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gzqhzfqey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/giwvqqofw.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/golkfsnlb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gxwnilkol.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gljdaquvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gleqpnslh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gognmaqdz.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzkdiaiks.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gcglkprzk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gljmruotu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/ggmbqwula.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gipnfvvcb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gxthcthcc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gfcmgccxu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gdlpmormy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gzmxwndwj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmoahxb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gmtwealbb.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gdwzpcqek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gyufhnxza.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gdeahfjub.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gceomzklf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gbniwyrch.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzapqqva.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gfhqfeogw.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gqrdfskqq.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtywuexhn.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gwzysmpbg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gghkgotwx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gpwdkoxsq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/ghmfqesrf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gmzlarhbc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ggwuylczh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/glhokicin.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gvtgcdmcv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gaxcwcgbr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/goghxptxz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/giipqokoo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gamjuxool.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzdxndobx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/grfgqdnvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtnlhdxdj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gvqqmtzjr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gnmljaifi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gwoutiftc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gilpvwxrr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gfbtgtmpn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gpmhnsybi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/guravoacj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzhlbshrx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gbmiicrpa.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gdrnqppcy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcvjuswii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzwuujdug.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/glaryijqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmqpriaua.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gwtaapwbm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gslzfeivr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glzqdidcv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/ggygtrmwx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/grwjezhom.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gthwpkfxx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/ggiaxzhct.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/guwgmyewo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvkknhhrj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gpplzttlp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxwgziflo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqidqgopi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gjjxzctbf.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gpwdvekxs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/galqbcoxg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/giaikrnfj.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gyvhjvags.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gnriujctf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/glkpekehe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gxarobinw.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gjxktddoq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grzausxfg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjdwxpkvq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gpdjcyoqh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gjgtleity.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/girgxnzke.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gjtxdldsw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ggdovrxoz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ggpobzext.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gsakosfqj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gfvultrum.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/glzzrxekn.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gmcdkjqqz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gdubcykst.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gdewzkohx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/ghijcjico.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gurekexvy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/ggsytrrfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gpkrtjwgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gpqdpskzy.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/geszxztut.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gqiffoxlb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gywwankfl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/ghekntgqi.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gaasjrbda.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gqghylghc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gtejwumlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/glxxardmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gdckhaggm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gitdlixzb.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gyosgryad.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gbdapkjmw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gdmacnvpa.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gigtmhwsn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/grlrzusrx.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gqjwiumkq.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gotbkriwj.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzthwccna.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/guomcvqxl.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/grwizyczv.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gyqpnpmik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gyaxxlsmc.sHtML


<!-- 参考信息 -->