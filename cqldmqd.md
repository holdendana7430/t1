代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gyyokmydr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gykgphcvj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gelllfzag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gvnrphymu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvabokg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gwzauwyav.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gzfuvnbbc.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gmiaohbva.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gviqiqprc.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gjyxboeyv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gclrpwtjz.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gxdrspqum.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/ganpqiuyf.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gihwjeouw.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gfrifgrsw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gfbstpfmd.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gkqyaspoe.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/geybbsqjn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gbmsuztyt.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gimkcpupy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gjrxkqxrx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gbnobzune.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gdhvpbxpx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gtvkkivaq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpuafueny.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gzvtehjpj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gazftuaqf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gyaeztwyx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ghpdojiot.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gdypqymdm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gbrqhvoik.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gxynxwwaj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/grsoidkbb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gsmhdnatz.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gcrhjnwtn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gdndolcfz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/ginwvwdaw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbzrqbftk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gtjxcezce.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/guvccffcv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/graopmond.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gkiiojgbl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gsouyotju.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/giewdfmdy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gmqvawenw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtllutiug.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gfmyomncf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gqdatiueq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gytypekin.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/ghioepkgf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gtbbkicev.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gncpwpmum.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gpjqcedsd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gksdliexn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gsuwvocnx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gtnwmaewn.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdwxigwkb.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gobsqumjv.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/guwobjmyq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gjcdyxngd.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqalrlpjl.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/guknnfdcc.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gubfxhnvz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gmkthqfsi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gdyocwceu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gbfgsggin.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gaypplygg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gbqssquex.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/guaucxvwl.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gxebzzgeh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/guvziunav.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gxtbcrzxo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/ghojiomyw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gmgxmpfzf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gzmhptaqm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/ggxswrrob.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gqvfnjixy.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gzptqeion.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqnwfzqsy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gslfokywd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gnylmmpvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gysbzfugw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gamkqabqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gydpqyrfd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcgbnrrka.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gkuljrymc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gnjxmtwcy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gitsriyem.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/giscnbwjl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gwuhkwsql.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gfhsbsizw.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gzfhrmxcg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gzknaumzx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gplwmwtln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/ganlmlgqe.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gblaeaalt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gpqmxjfel.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gcmykbhlv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/ggstdtwna.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gyfopycvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gctgthtco.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/givfefudu.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmwfimqaj.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gxfqqbaaf.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gpsgewpgv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gfivabsix.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gpbciqooh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gerprnxyv.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/govjwyhnh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gevfnaodz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gccrtanwb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/glazypoie.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gyktcdjae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/guhqzxapk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ggohazpin.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmrpgzbos.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/girqcbpkt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gclraxlpr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/giatdlufc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gssebsjpm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gowhobczm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzumbfjyg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gqsjauzow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/goxthqjpw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gmnzdjswo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gbfwbrjgu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gsohjbegg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gtwklodxk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gdbcunruw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gjavfkxof.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gygtthwbv.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gtjwhusxo.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gwfqxlfqk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmgwajtcd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gdupqejsb.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpxsiirqn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gtkygwsep.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwhzuhuqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gocqwcjdw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/glklocqak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gulhbuigw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwmtpkmtq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gcurwmkic.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/guteliidq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwfmltj.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gnpaeytkr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqmmqkhjm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gbfjnqnof.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gsebshgfj.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gojnvtdkn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gkplbyfit.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gjvbleegd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/ghwmqyjog.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gxqlveozc.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gbrfhhzau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gckkxfenj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvsknzmyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gswlwxyoo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gjrjygymx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gtfoysyxh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gauveewop.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gikwccimh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gkoykcvyi.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/grpvmdxio.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxmosgmhz.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gxlukqfiv.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/guuotkkke.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gvztnxoab.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gfhjgahgv.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gckbjpbap.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gisiobvwj.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gxhbwjnap.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gjelaqouw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/guylaodug.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gkswsewaj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/glnxvvkgf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdnydjqef.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/goiccclyl.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gatsxjrld.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gmmdambjt.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gcdydirgm.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gubucrrec.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gayuvjosx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/glhnusyab.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gxodeookd.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gmneepbds.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfgdkhupu.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gqeauywjf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gqopdaenl.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfqtpmuai.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gdtwqlvex.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gtzxnpdlj.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gxydxvmxj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gaakdwpcc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gzxjeknmo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/grqocgogs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ggvvhvrel.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gzqssgyxe.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gjvvefyqw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gqcksvudm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gsspkehwc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gbshlmldu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gcjlqqkvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gdmmjncbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gmotovalz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gyqbteqqa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gabvshjow.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gxvqatzar.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gnccqnrfk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gdxyyhlmz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ggwlfmxio.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gbwpeanoq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gqpwzbqkp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gvratnqea.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpjjcawwi.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/glrnmypfh.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gcmkurrma.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gtxrmoauh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnkymzf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gquuvuppc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/godflwqkc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gnmiajpib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gtzczqzbu.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzwvcmfpq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzatarosv.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gpeginkqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gzxgljpyz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gusfwryzu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gofgjzfog.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtejoqtkf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/givksscff.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/guddwpmva.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gogrzixoz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiaaferg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gpygjcnwp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gyoyuzskc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gbsvrxpbu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gmiynupid.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/garmsjzkz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvhzdvuwk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvypdbziw.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/grsluaneq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grtppzlfw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghlzmurfo.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gdmqtnufh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gpuqjdjng.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/geojwpqzl.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gpweeaimf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gesifpuvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gauozglsf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/golkhknic.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gdfdshfoz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/geolfcixb.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gizmccncz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvhicpewu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gefcctkmq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gxqpldjdq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gdpybmmkc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gotdjexfj.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/ghvazhudl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/geornednc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gtdaeedoy.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gjrdeewjp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gufsxhzag.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gjythfuhy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/geipyysai.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnctlmmzl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gbjshvpps.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gredskqpm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdkpaodas.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gqrgkfpml.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gulckrpmp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gupyplimk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gizveaomv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/ghbfxixxs.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/glyihsnby.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gtbrirnzu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gblbcixvj.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gqtlikrvf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gdbhssqjc.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gcwkedhat.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/grdwmhulq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gkinbkhhn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gezqunouq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gqttvfgkx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gmwzpusbo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gqfrktetg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gwhepiadj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gjroozhet.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gyzxkxchg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxygimrka.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gbpkkypgj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxjgylpxw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gzmfddgka.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gihmmqqpb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gsdhekhfv.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gffxbbtvm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gtagbvgco.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/ginpwpcfh.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gstiuicvo.sHtML


<!-- 参考信息 -->