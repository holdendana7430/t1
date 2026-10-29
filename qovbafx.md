代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gxawnakpl.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gmeucnpbb.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gwdtptven.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gmhyebqvk.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gzkouqbwx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gridwbioc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/ghoiwzuxy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/grkgsieno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gudjdmgat.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gkrictmtm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gdnbrrdsn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/ggfjfmadi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gnteirswk.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/grxdytzaj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gxgktxyxy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gjpxfunax.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gejqimwag.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gdvegivft.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsoazjvvi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gphroldta.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/grqhzwmye.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/ggykkdqya.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gyguxyegm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/ghfwdlsbn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gehspxwip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgodvpy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gajeqyors.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gwphbpspd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gceeteqku.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gvetgxevn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gchavnhao.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gzdufkckg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gqraregky.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gnboganfk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gyklxvyrt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gxvmzqqxd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/ghirrbipt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gytikrzij.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gwakqhbfz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gtetjhkmf.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gxrhozlnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gsadnpzrq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gsymlwsie.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/goxhiixut.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/ggwligoeu.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gckeztbpi.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gowxriptr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gthpennau.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gdpwhzvfn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhczxep.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gnyyvcyyq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gqdbecpym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzchdrwua.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gpmrcuofy.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gjalcpbuh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gdohabwim.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/grcmngcqu.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gqxxcipdz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gjrtaxdoa.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/grlrodart.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gszhqilkq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gvqnshgui.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/getugemus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gbzjeloqs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdjanubki.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gwoiwlcrx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjexsnaka.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gpjoelrhk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gjkqnrcub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/guinesmvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gdosfvdor.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcqrsxeop.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gskbsrrvv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gmhrvtlqh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gjkbtmueb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gtnekompz.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gvvvzoyhs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gqzmmdicj.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkfmenavf.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gobigqtzx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyuixbacz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gagejzpgu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gnysvovxw.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gmcutxphr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gauwcyamg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gkhtcznez.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/geprqjwoz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/grqmfxgqx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gcmijelxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gxytayqpn.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gyhvmhpib.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gzwyyeepy.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gpbyiypym.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gnvctcnov.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gvbgajlmr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gjatebvmq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gzwnzpwij.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gxbgdozpp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/geujrexiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gvlhnxvmq.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gxbiopfvi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/grahuqqla.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gamcrgweo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwdlvarkn.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gxiihqydm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwljpamjq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gdbnnmjpe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/goxbamlad.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gjjjiwcmg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmhqdumhc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gpzhobjhp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gvgrakpvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ggiqzpzyo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gfsystpzh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmexfjvga.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gbmzahycg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gfnzkfiix.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gygjaitjv.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gbdgmshqq.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gfyvsmbmu.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkkfkvoqy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gwshkmhjp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gxyjetjao.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gxcwwneol.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/grozamels.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gfcizoqzz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gjsttfupn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gttbnvdxj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gpcscsyek.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmspsbcci.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gwhqulemx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gikkltmza.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gddgutecx.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gzhbbvjfn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/glkmdcfgb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gqrydqcnp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gwhoegbnq.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gtjjandbg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gvfblzmti.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkftftaaf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gswbvbrhw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gfkxiptib.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gyseaastl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ggnyibced.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gikiukggz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcggnzxxe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gsikenowe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gtbahxqtk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkmvhgqaq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gaczsfkxg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggqvhxwlp.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gzqphjygg.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/geuoxlihy.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gydxpruiz.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggayzzlvc.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gpmnjiokt.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gerjauvhl.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbpqwigzy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gclwcdzcd.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gycdgwxos.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/goelszifm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gldfltjol.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gzraelqxv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gsaivteqk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gitawdpkh.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gsoxifvhf.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gbfjhynnj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtuzdmfii.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkvaywxqk.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gfopknijp.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gwxaaykso.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gcmnxvyjs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/ghbjpjgcy.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gybfiqgxw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/ggzlordyf.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gslrlpfgw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/goksnkdyl.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gsbdnvths.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gupayeaun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gsuoxhnxf.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gijokugfj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gabdghzzi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gkxaxwcpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/ghhztpjrc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giwbbiljt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gjgrkbtna.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gmukpasug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqxdmmcnd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gytfngdqa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwrzerqmv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gcoprpvol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gjvcsxbgr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gnllqhbak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gmoaizudn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gjhihurnd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gjuuychds.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gksfjxnhy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gzlpmumrr.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gytfnjhxw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gntqchkan.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/ggrahmsau.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gzhuslszz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gphzscouy.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gbsymfffk.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/guoujmnwv.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gpgrnuajp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gsisbiery.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxcwoglje.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gbtfirdsc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/ggfwdnmpz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gaygdvstv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guwxvkdpj.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gxkgbdgxc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gnsymqrnu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gdamthfsu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gzdkylvzw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gtwsjolfc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdwkmtsfu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gyltfjeru.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gyrujybra.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gohvokaho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gflvvoujp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfdgshzbj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gciugtavo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gsqsbkoik.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxmyojqvo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/grpcflaql.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/glkytavyf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gkjboxkso.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/glyvxznxl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gazhnfirw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gradstqvo.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gxejcixwn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gldkwqqod.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/grzkmoytd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqoeckofy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gvoofkqtf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gxlkgbuqu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gbhazbuur.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gzwrsgybi.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gyflwubit.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gysjwfuhn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gexsdvrlh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gkiucjbde.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gpnfrkikf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gcrasteyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/glyfznpdg.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gdejkpfgc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcabgxxiq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gntvhdumv.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/glsvtwgan.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbvfmvqxe.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gnokmbyvf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gsfnvcccl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gbjtsvwwi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gzffrqjnb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gamnmtfui.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/godyixpeg.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gcggqswbj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gwiityyef.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gyuvfhcxx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gdinyesmm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gfimeficj.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gziqmlzwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gxawjebuy.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/ggigmmqog.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gtcwstoka.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxfmnyabs.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gzsksbyzp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gnraysuei.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gufzbaxrq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/goupjjbyg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/ggvgngrec.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gqgfvwojw.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gsknoalgj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gfomueqba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gjwnzrizx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gdvjiyxiw.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvwdphqft.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsxwrnacr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gviqgjiwa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gnszoqztc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gnbaafxfb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gilypoqoo.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gnxumpzlf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/ghacdueyd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gbdpqwjia.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbxvtgtok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gfjshpkua.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gdgvflwqf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guqqmkgrr.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gtqxmyhed.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqtlkvj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggpoenaln.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gphftoasi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gwocneczc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gahevmref.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/grsccuewe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gqhxddhjs.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gmpwfucmz.sHtML


<!-- 参考信息 -->