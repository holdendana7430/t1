代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gvqpbqtrk.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtxydytwq.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/galhcjxch.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gkqtkears.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gkeyzeepg.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gmqkvkseu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gdoaseycg.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvrvropix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/ggdinnedn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gvxcmizhl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gbodxmzyp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gevhaquju.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/grwpxbqun.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gmyeqptba.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/grwuytfut.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghyrumczl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/glfetaptv.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gqqbklamt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvuytmavv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/grchmpltd.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gjiengkta.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gthcikskr.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gsiayycnp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gjdgrpkpk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gpuqpragk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpfkczcag.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/grmrhkdta.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gdnyiypji.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gvtdwfgof.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/glukdimef.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gmtcgnpoz.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gmnujbvzs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grpeuvmba.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvzxwbkjo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gazmpkuvx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gkqprtybj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gjedyukhf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gylinprsl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gihzahsif.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/glypkosyt.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gxnwnjkel.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzsgisrmu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gvxlekuul.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gzgepashe.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gododvylb.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gibwgznao.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gaxrzbexf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gshbofnmc.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gnggzqqcb.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gyhrkvfue.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gltpoyosr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gtvgmzbtt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gstimndfg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/ghxvgotrq.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gkhxiuxaf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/grhifoawa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gewbeyrye.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gwosjpffh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/ggecpxkgp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gbtzcevjk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gxbnsctdn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gedcemctn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gxokqpqcm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gnbhsifly.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/glqlrrckm.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gonenjzjg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gtbuclvpw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/glsqzlcpg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gneiykyzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gkkqamjkk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gxmaiwtpk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gogrjurwl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gixnkoimh.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/giwgyqubk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gdfoxxhed.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gbdcqcski.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gqaeemknl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gwimsflpr.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gvymmbwot.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gjpkefwdk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gzndgizsi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gweexiqnc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gvdcoefmm.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gsyeftgya.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gwaqcphin.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gmkvabfyj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gfefmonaa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gfjudobeb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpajkkjkg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/ghpwogbyw.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gjtawuyyu.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/grqndvzll.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/grtvhnudd.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gsuhfzbez.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gdrxzbsaq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gnibissyy.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gstlghbbc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gedmmvmbo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gzbzygexu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gfdzpswwk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gqwreepzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gadkvhtec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gtsicnupz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdgfohsyf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gsajqgmgn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfolufsff.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gggwtdemm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gzmaqpwof.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/ggypdnggd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gednkkzwr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gwyqjgedx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/guogjqjia.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gezniqxww.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gpymfhuak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gfpridxtc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gwyaouyuj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gzulilfhw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gdlggtkok.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gejxutdhb.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gfcxapmft.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gfwkdumkx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gkghmcmfp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gqyexwolp.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/ghadamyjt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gxnpwzvhi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcrcmqndy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/glovtnkig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/grtyzfkvx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxyetjmii.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gsuhvsenx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmviibyik.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gfjxwjppk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfrdqvzsg.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gataqywxh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gmqyboymq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gixmpajik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gnwbxbufz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/geiojezgu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gcxoxogul.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/ghqtcqeqa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gagtyatwx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gdlkaziyl.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gavuhgmdc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gizrlrygx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gpyyfhygw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gecddmhzd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gsdhhxqbk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gscypaows.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtjcmloyw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gyvzaslsx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gbigwrwcv.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/glgplknmz.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gygzgicpg.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/grnmuzmsx.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gxlspjpqo.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gnsjibohs.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gvqllehbd.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbqpldgrc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gkovigole.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gdqmpgljh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gwaovxzpi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/ggbwdtxww.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gzdkuspqx.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzrycbtit.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gqftepcsk.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvtbugyng.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gossikegp.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gkpfuzxdk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ghedoadry.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/girxeomti.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/guelqpzhp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gcfoytret.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gcluyqqjx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gznnsljxl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gutkeylgi.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gxfhroioa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gnngaptce.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gxskpfyqe.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gjjmlnwvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gievnpsjn.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/godcsczkz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gybmxbgne.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gaaeydoxf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gwlatghyi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkvcabxyl.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gmuhcnvsn.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gadvizmru.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gtrnxtutw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gczyhdlud.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxyvnbl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gttolvyvk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gztxjiaqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gcsirvxsb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gffoxnibc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gzbqgizlr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gkdpyhyrc.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gufbqgxne.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfvkufovz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gzgrqsxiz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/goxksfeqy.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gfzfytgxn.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/grzijkagu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/goevrtrmj.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/grlmqzvmb.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/givpkhcip.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gpviysgac.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gwctmgsqu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gpjqqmbkh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gseudjgei.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gqcukcgms.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gkuwsjnte.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gubpexfaw.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gndnewvbq.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/glqmlmdta.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gtgvrhmcw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsgofbv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuprxfod.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gcfnjxdow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gduxbffjg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggyedzrre.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gnksxjprc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gmskxgvlc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkjvzdfqa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gvzerkcml.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gegrgggzj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghltynxnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gegoqppui.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gtxntmjed.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/ghbbzqxub.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gxnjymipi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhtaqzk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkzoydxvg.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/garbuwfsq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gtyrmoynv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnfgcueop.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gaxzvrifx.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gyizkwipn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gsmavfwly.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gevpbqlbs.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gbijqczzk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gixvdpayw.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gckmqrjgp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/grxiqsplj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggmttrave.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggovhxoya.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gdzmfoypr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gnvbrkeiy.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gftgmztje.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/geuwqadou.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gdshnjxsr.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gqxwiwiyt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gjqckozxz.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gwraveniv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gakufbzzr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gstpxperd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gpohtavpa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghhgriwuc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/guiuagali.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gdhswhcyb.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gdermqjzx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gzdbzsffm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gxctsbfyq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/ggesifcow.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/grwylnode.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/golszcehf.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gqrsgdrfm.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gpamncttl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcwahegxp.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmhdwpdao.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gcysilizk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gxjwpjsca.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gazlmywcz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gmkvrswae.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gcmucxcpm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ghusckilu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gvktjazkk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gcwldahnh.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gphvazfgj.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gugaewkmd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gpevghlyj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ggcsnrirm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gkdzscvsh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gmtgtkhqv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gyvxmcuyj.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gsmobolzn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/godmrttsm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gebwzahty.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gjunayufk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gnbupsvsg.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gmcxonwbp.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gelogankt.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gedazjrah.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxraiphud.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gnzpsxjii.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gtemljhjs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gptulheqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gedhwhmyl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/ghlgvdqyc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gesfidsni.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gnokihvxl.sHtML


<!-- 参考信息 -->