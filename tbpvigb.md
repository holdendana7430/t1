代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gwnwttmlt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gemgssdpg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gisphlbvh.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/glnhpatuc.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gioxzlmwp.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gdowtzkvz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gnlyspsah.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gnwdsysfb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/ggztmtvxt.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gqgzttlfc.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gyyzpdrqm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gqcxzrmoi.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gihdldogq.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gswhtvzit.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gkykwhsnq.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gqdyqctsf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/giaupgegx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gmorqbprw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gzvynbwgz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gumknyxrg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gwuggeaas.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gruuoicmc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gezddxpdb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gubcoiapm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gxubscglq.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/ggoojmkio.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gjqjpreek.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/grywrvbpu.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gcvhfumyo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gyytuulpo.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gmpvxdadg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gruptgiry.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gpkcilquh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/guzhxufpe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/glqjiezji.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gmftvouvc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gaziivsbw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gqkrzxbnp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/genltymfq.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gwcpxhtoq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gptazixac.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gtpbxnybn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gwicsngbh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gclukbjkz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gxghovslf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gchvqrden.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghacmyhih.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gglluxltf.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gqdnrrgpl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gmzoyhvjv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gqntcxlwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gjdlhmhhq.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/grskuusxn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/glhwxggxl.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghzmaofbn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/glcgjsbmw.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/ghrzrtaza.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gbbfpcmur.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gcspuwavy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gnsqpnpux.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gpowyqfmu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gpwetnrut.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gckrvzdry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gvyhqpepc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gxivtdmbu.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gdiynddit.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/glmkgzvit.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsqwihrbg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/grtrjmmjc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gbuzwkgrn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gudzokeux.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gseatzsqp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gblqtektr.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gudhneylj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gcsrbhiko.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gllhmfjlx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gpgarehnp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gcuwhwasr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/goqkygbmp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmyscdoig.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gleybrwge.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gyexestga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnmbwszgt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gptcjwott.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/ghzeswsks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gtwkdgrpk.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfgxwkbst.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gmeulhyxd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gewgkdgus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gtlrytpob.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/ghdvnykne.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ggvhllnkj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gmyybjbsp.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gjbdglmmg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gqcwappzr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gkzdmaunw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/golqobvfu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gsmnuczwx.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gebojeojw.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gajwiqwpv.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gopmloguc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/grbmerysu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gumjbhmpr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gfnukqxkg.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gqmmcvlkx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gxkmguaoq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gpevycuuw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/givcdmrgr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gfhvynezg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gdondyocl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gvcpxdnhs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpsrhfnxq.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gauyfhzjk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grfjjnosk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/ggziricgc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtulztqrx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gkutnvync.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gvbpscuch.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/guqiqmxtk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gwsxgimjc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gpdlckrkx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gupqnkvnr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gthqliklw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/guijzdddd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gchmktajp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gmcazldxk.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsyzkcokt.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gesjymndj.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/grutasmgr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gszxacdfq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gworegqpk.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gesrbtarq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/girzmuvry.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/ghrkkdmht.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/glirwigln.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gciwcyyif.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmbmtievn.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkswcvmdn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gumtlkrnh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gstceaeom.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gsqwhvpyz.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gouwsltuq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gbnjfvhqw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ganxaopuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gktnacied.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gywybtxcb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/giumrlifw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gxqnjiwvf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/glragbcvk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gyxamkxuk.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/grtzbzpvt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvkcrtkdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grjmqqjnt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkeiffgsz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gixeudgch.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gcxlepotw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ggpcpslhf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/grbnffimd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/guqfwlvla.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gpxgmncxg.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfcnbjbkh.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfenjnciq.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gknqnabqt.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gphehouqx.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gmtmxpbcr.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grlcgyrxr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtymzuldd.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gnnnjrkkq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gdqszbghu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gappndpln.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/goqlqsuex.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gsrshmlay.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtqqptdix.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gchlpjgwg.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/geqejoskk.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/glsdlhdip.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gfnvtcuxc.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gwoyxxbqj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gbgviajla.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/ggqrpdcwv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gamjjhmlz.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gbabniuxa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gsgeyibkc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gkmtnhsnr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/govjihpvg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/giclbaoye.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gpqwxexyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/giqmuqfrq.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gbkxvvrfr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gnkaviyjr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gdhxduuge.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gotvfwmpd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/guzyktreh.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gzokqpcqv.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gvboksksw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/ggwvzvcjs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/ghjhvmpgy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/glyphjdoh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gnbdvjflg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gpvaejyqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gbqgnurmr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gttuyhkdg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/giexyvlfx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gvmtimypy.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gcodhyvpo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gelouqcxh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gkdfehiiq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/grhbndzlh.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gzgizuujo.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gyisburei.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gdonerfbn.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/guvegwusu.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gwwomvxva.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gnssffywk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gxzhcjqbd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gtjimmftp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gngwhieeb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gjikzyjuh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gezjmphre.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guevmsoor.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gqyhddooh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gwrkpawaw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gswinxwim.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/goruniqye.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gyjdbplkb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/grzqqaedq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggwvpxltf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkyjhrfmg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gncfdbrct.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gukqndesf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfbalopos.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gsghomqjd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gbosnfzbh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gfjqdxhyt.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghtnjckbc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gkklyrmhx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gbiqkmbav.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gilhtftyz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzjjghrzz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/glpdpbxfh.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/glhdywllf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gzkjugfvx.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/guyflufhp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gqstxliiu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gcmjkjkij.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/grqjxlsjv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gheegoinn.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gjdupvkyj.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gvtirkawg.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gabztnjqv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gnjjxhzfj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gffyhyefg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gtioomcxn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/guendjklo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gqxryhidr.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gntolthjj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnbzsouuq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gjygzzunx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gwcwnsgac.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggygilyks.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/greuqtkls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gzojnrwbr.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gykxhqgku.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gldfgbkpf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gykbrfvhu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gullgqjql.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/ghzzxbelu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/ggjkvdcto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gcrifyzgu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gruphsyhu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gxzvlmsjm.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gkfcxccir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gdqfkekul.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gbgtlbtiu.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gobbnhttt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbkgphjud.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gnxladfff.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gjmfhzhmp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/giyajusha.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gpdfspjga.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gwomlauhk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/guohwidli.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gvutsuriz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gyzphwxds.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gqafpfxzm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gsuufknsi.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdrcjdkql.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghsxwtdks.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gtzragosv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gqrcfsuut.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gufrxrhqj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/givosiyaj.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gqkwamjwz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/glpwqwqqu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/guaktqbfu.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gttfcjabu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqsfzwll.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gkaxsyxgl.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gbskqexqr.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gxmxxemjk.sHtML


<!-- 参考信息 -->