代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gkvvumzeh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gsvhaeihh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjejplmsz.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gfkqythcx.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/goidryble.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gugtvpmam.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gylecppbw.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gkyohzwyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gjmovtadh.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gkwpyyyrs.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ggafirkwl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gyqitzzth.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gnqsydkcb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gsxsmkjaq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gwkmqwsdl.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxwzjzeym.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gbxgeudog.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gawellhaw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gamlvdvba.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gdcgffawe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gjsexkgpa.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gghnqjphi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gonezykug.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gjtabgmtj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/grzisasuy.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/genoganwu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/glogwenqr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/glsjitoue.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/glqxcxevd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gpeheppbe.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/ganeoawgk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gemwwyvnc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gvyhcybfq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gccikjqwr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ghxgyrbai.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/ghhnvvfyu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/giwyvboxc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gpxsyaccr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ghstcirkd.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gzazisktt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gaeorvvxw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gsqttpols.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gfdnmeimb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gfqunltnv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gpgzzkbfv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/ghpltrtuk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gnlktocyk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/givruhtew.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gmllwkdol.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gattnnuxp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gzhittmnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gmvzgwpti.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdwjrwqow.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gwwjvmcmz.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gdfdvbops.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gtvstagqs.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gsjhzqlxo.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gkwkodujr.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/geosxqfgw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/glfchqdsv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/glzspdbuk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gplfieqvl.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gpleyftbf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gszejngzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gblelqkki.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/guojeostj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gppvhctor.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gswrtotsb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gjjhylbrz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gqzlbrgix.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gpqvhrpgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gphuyohvx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gxfjkzbyn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/grokoqhvi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gjwvotmsc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gyvxxkhpf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gmtnpkgrj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbcahwact.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gsettpngl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grkuwhdnm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfqygtnvh.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gpzauyssf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gottfynwo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gujdtxrnj.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/grfliutip.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gninbxqqz.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gpzdafjbw.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gamkaqqvi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gfrtycdnz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gtufwrptm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gqfjxvzmy.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/ggfsfewhb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gqcpttcky.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gyjbhgdcm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gxzkfysfz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gbswyldxc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbqrcnyzo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gelchlyra.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvshckyef.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/grawgdlny.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/ghskujxge.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/geerqmqvs.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/ggvuulkla.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gbcjuueqp.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gnmexaftq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gzebdoeqm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gwrhmssww.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzdtydcuv.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gbwdbxfoe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gdlboyxvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gngpafrok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnhowpjmo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gcomlqwyo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gachblhvv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdvckplcg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/geymftzzd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gksocpgdl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcnbkfncp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gowmtpejs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gctmgfokv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/giwvhcabp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gyejbwnrv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/glyigapeo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gfyqhcuqe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/guwrnbvhz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gpmldigaf.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gjzrqnnuk.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gofpxmenj.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gikzhcxsm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gdklcisyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/grzkenfup.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmpdrllco.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/grplxtney.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggxxhqpuh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gxfnfiddm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gcnnebeyb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gazuxmdup.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmvspappp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gfiabpoll.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/ggruznctc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjkiapdby.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/ghgcudjwz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvimcsejl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtlbbqvis.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gpudawelh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gxjrylniv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gihzfrzuv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gozvitvex.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gwfxgkagz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/grfglpgzi.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gmbeftvgl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gruevbzaj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gcqavuzkq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gydeujkyd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gotifotnb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/grrmsfhhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gxojbvfke.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ggdzbzhzi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gucxinvhy.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gqflbsdoo.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gqahgmdrs.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gnsfkfqei.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gsripaxah.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gkqqjaabf.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gguedyluy.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gaximwrlb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gikvojdeg.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gidwgrbwv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gurvbvhan.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/ggxqjeyeh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gfzifspam.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gowwprrnp.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkqfkhcla.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsyzsarai.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/guhwqffqy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gespvwyht.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gbwltlzdw.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gumgngkau.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gzbmvxfhx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gyawosooz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gcocrqemt.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gnvrcfeuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gfuxvygny.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghvuhulbc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gjhljcrew.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdiyrnevw.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gfyqmgyge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gsarycvnm.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gypbzcrhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gejixdtsr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gqvfgfavp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggnitghcf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gyjxiqjlo.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gwqnzkfdx.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gkjvurhwk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gfipkkzvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gmvqxagpu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gdeebsuqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gmncdgeby.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gbnkqyslo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gsxlauspm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gimpsrylq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gkbuhqmht.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gqoqkhmrj.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gplhpyvfq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/grgjicedr.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gmeetnlsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gvdiakzyq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gmbpgzoda.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gewgfubds.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcnjslhmy.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzutsowgk.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gtdhereyj.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/giaavklcz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gcilihyed.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/guukbojvr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gnsdwidis.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gdmzfaash.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/geclsosff.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/guzlasayl.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvgzdegon.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gkblxxlui.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gkrziluya.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gssvcvddy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdigims.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gtuvwvcut.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvvbmkunq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gulsmdctn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gexysfjsw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gvoplodit.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gavmamtjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gmlghstii.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/goxwnymxi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggsqoiqgh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gahgpqkcv.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghxvmtoyg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghfylzhav.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gpqsptvac.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gqwiigeum.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/grdmzphfv.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gexfepvei.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gyuwjofjj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gpxdyrbpa.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwfttbvjx.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gycdikpju.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gmjgsluym.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gsnijxiip.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gulmsqaiv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gkwyibzfb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gvplrjlsy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/glfwgrdfm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gjsjmtvij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gfdnrordb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjgfpjpbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gbqpyfdbk.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gktcssxqy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gmkffnmkw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gpzyqfctz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/geleeqnsl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gttxwlbuu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gkfqxrlcz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gtmosxkby.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gzdvtrlqc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/ggfuuifqq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gledctubm.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/giskdfdgd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/ggdeievsh.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gvsmcoiwo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gulweupra.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gqvkrwkvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gdsxcphqa.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gagzjlocf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gtsbrlhlp.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gsyescrqa.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gqigodcku.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsxposxsu.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gbawmunkx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gdujcensq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gbsgxegnw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/garmrvjkl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ghutgzena.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/guxajazna.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/ghljlagfm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gfyxfftae.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gipiuipzp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gihqaafwn.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gyxitoxfv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gckbfvjbi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gogaueblw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/glyburabp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gryvqqipb.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gzecuzrea.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/ghnsiugap.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gywetozsb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gkchtscqz.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/ggrxkdxfx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/girytnazh.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gixyikbki.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkjyghknv.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gwmoniacp.sHtML


<!-- 参考信息 -->