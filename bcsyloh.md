代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvehwqzi.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gvtfuoxis.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gwbhhfmhv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gggyzqmsq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gmyqfitnq.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gqmlnllhq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gjlykhzem.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gcvdtvgoz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gwgjvddyp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gpntmoybn.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gaehxkupr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/ghvsfhuot.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gbojkrgnu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkxuedvo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gedmpydwl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gyvlohykx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gjhznchhn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gbbfkzawf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gcgvbeqxx.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gbmpicnyl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grcxqctqo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gjqjscgxm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gxebluckx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gijcxcvps.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/grntvkyuf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/ggdcwdivd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gkgxkcwyp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gbifpxjil.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/grcoiekuj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gkjseovfy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gtotpzyuy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gkdwzlouy.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gvlgrnvud.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gbaksqcuj.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gnpztaotf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gpdnigtgb.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gsjjwnkka.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/glmepyvwh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gboitysbq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ghuennfnv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gjsgmkzzf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gwlinjmnj.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/grnzjiykf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gecevkrjb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/goxovmaen.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gludvxdjc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gnadaguek.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gjlqrxaxb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gksjjckqx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gukfvwkfd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gaeanxwlv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gerrhmudf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gsdtrmidk.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gwhquauuh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gjgedmezd.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gxkruwwhe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/grqsfznke.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gestvuvmn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtlphgmaq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqkxldsuh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gaxymwkye.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/guzcqoesp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gkkemdsub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/ghovcbnth.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gcgpkjckm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gvhpxzeew.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gbkwdoduo.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyrruseaw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/grfvknjyu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/grqsntjlm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gmkbnuqan.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxfasixuv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gadbfbiba.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gcndpfjkb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gtpeduxlg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/geuexnxpb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gimkomvhe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gfifcsofh.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gfnczndvw.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gahiairjb.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/giyheaoch.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gwaxhuiyv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gxmbcqjue.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gkvizjvgo.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gmbyqbyff.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gparduafx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ggedhdxov.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gtathzcrg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gxcmqcwhb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gfskjlftz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gupbdkdxg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grmbdrava.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gyunzefpz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqikuxina.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gjnipzkpn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gtxwskxgq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/geiqcequl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gimfndtao.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gcwfrkcrz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/grrjvcspg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/grkrkdxsy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gkdibddud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gjikcyymw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gazcorsuc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gblaqwgwl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gannmwigf.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gtfupknrl.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/ggmzutrhn.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzphzcdvf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gkalooyie.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gqnsrjvyg.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gnqmeybqf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gyahxzlcy.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/guhaekwhw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gusdouixn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gnhuvhdvm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gqdrinmdt.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtxngazne.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gbrdelfps.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gllhsiigl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gcxawuqmn.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gepwpzbnw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gkzudgvah.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gyispdcls.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gcymdyrbp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gouaipoeu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gumtbtwcq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/grrpuivgk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gqsgixwyn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gyztkvmjb.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/glqwdkbuw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gyczefuuf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdhgzaext.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gyfuhptvs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gpxvzlgrf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/giixsnufr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/giwxfhpig.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gpdywltso.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gsmbvgzti.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvubyvdxt.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyoujveti.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmxlzckpu.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gklrumelh.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gjyvvysdn.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/govnnwmif.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvuzdfbjp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gmukhqjfa.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gyhedwgpu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gnvpbyfdq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gzdyxvusr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gnndihzos.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnpoqtbhm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gahucrdmi.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzmzsmkuj.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gaizmibdn.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gwbvmgkci.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxqxzxrmm.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ggybswufm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gteermdzz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gqrgcecxw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gerjqzmzy.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gqzmfwoqs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxnavcwtf.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gircieuhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gdwscoxfh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gpjifszoy.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gsvlqpgxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gqjpqkwil.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggvqplsco.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gnmdvdmra.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gyojsyheg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/grshdbrdy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/geloxmvpg.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gleftzpql.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gcppueeme.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gtnxkbuvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gcqijfklt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gtneriujb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ginbubnhy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gncjecbhq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gggrgdonz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gxtjfzvmb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gftzdbtmi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gqcxagycc.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gozckvpdc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/ggbbmsewo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/givuufpqm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gpaehpduv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gucfpuaqr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gbhhyojay.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbuuwwilj.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/glowtmnxm.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gystisgek.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gmysnchmm.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvlnojrzl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gpdiceywc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxziilbqm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/giwbhzamt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gsvwweyof.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzbpjybti.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvhmlmxot.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gsqqchpkr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gjndmuwim.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqmikptvm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gcxkaelbu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmuexxowr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gbyxvlygh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gashiuiyh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/grrxpzcoa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gftoamvgs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/glpymdmtf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/ggublvyqi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gogpavtag.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gglukxpgx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyywtvrxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggbtyvllf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxfskdynk.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gyyfkgpaq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gihalhboz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmyjaqcaq.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ggzcsihyx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwmyptynk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/ghpjhxsxi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzvwjnbgv.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gocaphdrf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gtmgrpfow.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gfukzpetk.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjbxpfaam.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gymdnlmqv.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gqpqqgcls.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gyindgyig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gqigniyjr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghadvgfov.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/givhuvilj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/guxgausys.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/glexonwwo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gosmrrsec.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gdhnbejkx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwbtofj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gajudinmw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gspyulhyg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gnimbaeuv.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gjldgqjbn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gocavmgdy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqmkzfjdx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gwacypwfy.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gkkzomadc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/glhcxudjr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gpipsixvk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gabwvedjo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gdxnucgcs.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gwhpmqhzf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gzwcugxsw.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gvkijiaez.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gvpvyvnqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/grhkxrmaa.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/greozrxcw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gqrdddyxr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/geonblwjx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gtmwyqqmc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkpcoeghh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/ghhgjackm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gjkoagsnj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/glozfsyow.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/glsvzrkzu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/ghvmnbnzv.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gsurfwaqv.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvnwaegfk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcnozvhjm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/ghchmgypz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gqjvwvtln.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gwhgnfeyo.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/grncrcllv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/ggqewopye.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gkvaxblad.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gflbzfarr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gslyisjmr.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjbxbhexf.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gbsoricdo.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/grjouvibm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/giiqpnamd.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzvoqtm.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gxrbnduaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gjqizxvzx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbzcbnavx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/geszyatkl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/goisokovs.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ghtmblllg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gpskkuvsh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gximdshqx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gbfbtbxrx.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gjdgbguxa.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gcrxuiemv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gzdjxsrgb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gkwvckrus.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gmdcrsded.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcldxqzbj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gfwyanrkp.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gjzmnpita.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/grfvvsjnu.sHtML


<!-- 参考信息 -->