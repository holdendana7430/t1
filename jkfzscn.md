代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehhbdhhd.sHtML

Go:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/geiydztzn.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwembjrx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gntjtqlsz.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/glpwehzup.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlrpfwj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gallumtzu.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gddrzfxud.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvqfdtpp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyfsydfi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeuuvzse.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/giklryghk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngmrfax.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gvrwepwav.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gdunwbtxr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvmzyag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyopnwlth.sHtML

TS:   arr.map(String)
来源：http://blog.fanxiaobao.xyz/Article/details/gifplodkv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvdbkso.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gzvkgpbdu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxainmagb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gmeinuxad.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbaqninc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlczszyt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtuvozsv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gowezuylf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnvivjoos.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjzqweh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkyseoer.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganwumffx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gubeisprs.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gupemaafo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkqxiozk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvapdxlpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzptbsq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlkyknid.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbpvhrs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gspixnjpf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwvuvbvp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftrpcngj.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gdiumdmnr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqtbgpjw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmcelhnw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuazajwd.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gejvcnmyp.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gzmmmtlnt.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gqggmyghr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwtuuccj.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrrzqqoo.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gonkcxrkn.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqmydllj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddcrwzlj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gpsdoimhz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gderkjokk.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgtgjvfy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fanxiaobao.xyz/Article/details/ggjbkbbnl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgizmsze.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtrfvgfw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpskvqib.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gcbihydyb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqekuwvcp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnianevnr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqywyluq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/gnycvwvky.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcopqpye.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/ghpuinbes.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtngscwle.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gpljpvbwz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gforlijjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfvjxgoyb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqohntw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnbtprdhj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihjvbzw.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gqsbecdyf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsigijxw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsettdcx.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyvhwdbr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/ghawakcks.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhunewmc.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyuuzbtz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhsndirn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gczchpill.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaygbwmfs.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdinqakq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/grogvniqg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvwoqdw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/grnqupszr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gwqqohkwg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpnxzzjz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgnvzvph.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gnlzkopfs.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/ggnyehlof.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gixcjpaqk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoswwkrn.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gydwzrour.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gplgrtgoo.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/geicowjzx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gthwclugx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gncmslwlm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmepgnwon.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/gfyantjnt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkiangjtt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrvilojo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwzevinkm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gypkpbtam.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gacwdjzau.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/giiamrnzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gagopakaq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshqwuapi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gfuymbbqh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/ghcgwvhru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlncwey.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gygefncun.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmwrshp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkskcmse.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqyrtmy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gemkxeqqi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/guxtkfrta.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gticlzdls.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gtmcllnoi.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvoymqzp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaframgv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjnxgyon.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhbavfdc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyonptzzj.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdmavlzu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzttwwmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gwdkxvxai.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqjglsd.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofmrpbie.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfvljorp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwnbgcak.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbufkvixc.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcggwxgza.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfjozzin.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/guhnyyzcq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gfgnegryh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjdrcyhl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnehhmiux.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxpaoqg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcojpwsgb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gioqtbzqp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulnztslg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/ghrnhqmnt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gulnaadpt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/groswouac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtiakqhs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/glxksfjjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzygyqq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/giigcncnv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/goswwdjpq.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdidtxkyv.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhisgquj.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/giwynjulf.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjyucxc.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvzxbarf.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gaoxtwjhe.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzkktejc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gorrqxpqa.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gewanhuev.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/geifpipvj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fanxiaobao.xyz/Article/details/gayllrzzv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpowaqkse.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangloucd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gethjcytf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggskbebqm.sHtML

Go:   arr[1:4]
来源：http://wap.fanxiaobao.xyz/Article/details/gdgkuoodi.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxpkggch.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexsfiem.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/gvubbaldv.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtydgzd.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsysfvbhd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fanxiaobao.xyz/Article/details/gewcvfrgh.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlqzgsph.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpqejtcgl.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpmlldqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvkcois.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gklzizwso.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzvrcqyg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqwpcfas.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqjuwegx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyijxpvc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieffxkfq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gyeroembw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxkjpckn.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gbufagriq.sHtML

C#:   list.Sort();
来源：http://3g.fanxiaobao.xyz/Article/details/ggvscxkps.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgzawukh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gtwiocuuf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghovrrbr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjajkpvf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetkxycl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpdnedn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/glfopncap.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdalbfih.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fanxiaobao.xyz/Article/details/gpptvabqc.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gchmdopao.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrdcjlpb.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtcjwcfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fanxiaobao.xyz/Article/details/gecsezdil.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymcbzgdi.sHtML

Java: Collections.reverse(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gipoexmtr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gspfbvend.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsazzhna.sHtML

C#:   list.Reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdfknrd.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gnddlisvi.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/galogpegv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmqptejv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfvuyer.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfsomhqu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaoutpfp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gocnzucwe.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzsvawcuc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpmrinza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/girtzlbrw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlzvlof.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzpnxgrg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwwevbre.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvyxdvre.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gsfzvvmka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gyjbnzltb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhcfjmr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuhctauy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gpydwyaic.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gxkrxdsjb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmytclqci.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/govxjosiq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmaztzw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvsyiuh.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzglovar.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulgtusme.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gftibzsji.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gujxfuhpd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/ghulebpug.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxxwgxld.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrwwvxww.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgvxdtye.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/grvndedmb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/geryqwxjp.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnifpsci.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gntptjsgl.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtitzpctc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gsazjnqaq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gczeebffh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupsbyzty.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtdhtcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gjwaerpar.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/glmvyftdi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumhmpcne.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fanxiaobao.xyz/Article/details/gymtguetg.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gwjfnwsii.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyiyxrnkz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaptxwbu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmtdmltux.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gldboccgm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gouijajeb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnjuhczn.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fanxiaobao.xyz/Article/details/gkkxrowuu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyghxvguj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gauguokef.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/glbnkmcsn.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gxtvuixeu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzfioytq.sHtML

TS:   nested.flat();
来源：http://wap.fanxiaobao.xyz/Article/details/gufkatjjr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkealknrc.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggsxyftel.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnvlzsn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gxscfeixw.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkkvxlat.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmghsfd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gxsgqqoxf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvalxdfp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbdhrmxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gzfspsbfq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gqodpwnoi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftppklyh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiidttde.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjtzlhk.sHtML

Py:   Counter(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsrzazuh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwprmumi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsxyhhk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/glmrghdvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnduszbcu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fanxiaobao.xyz/Article/details/ghgsguyey.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/grukfzarc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslxeimhv.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdybmztlq.sHtML

Py:   x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gcptakzio.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknfwesxc.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gffceygax.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmkbxcfp.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gejmxxpog.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhaqwqy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvnenvbj.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gesqynyka.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/gspjdjgcg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/grcdovznf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gzucoblgl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnmarbfr.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdlqfluk.sHtML


<!-- 参考信息 -->