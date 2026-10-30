代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gkjmwzpiv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/ghzpfeska.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gqlomlptq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/geukrekeg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gaazeikkk.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/grleayfdk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbbztpsuu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gbizzufgn.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gthmialsw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gskvklhrg.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gxqgtkpos.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/grvihomyl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gaqxsffzp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gxsllpxqz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ggfezxjms.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/giggunxsp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/glzjtlbdz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/grakgsymd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gxebbqlaa.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gbjudhhlx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gxspukqmx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gpjvfftti.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gxgsfssnv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/ggupgghim.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxntyyyxi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gxwvvtnwy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/grlmdxzje.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gsjqohfyy.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gifqbdony.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gkhncmxsw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gjiijyjap.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gmekbzmkq.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gocquwebh.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gnzilsunv.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/glodebmyu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/grozpsort.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gbsfcgjgp.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gumznfvrd.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gmxxcmbvy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ggwqpgzvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gbhrotrgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gnvtsmoph.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/glnxhcjeq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gadnflzvc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gcaayoazd.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gqvghzgko.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/goddcfunq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/ggeumikhd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gucreniqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gnslcyfdq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/giyosnedr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/glsuhwmaq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gndxnfutg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gtzcocuer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/ggkiehasl.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/guxjnvyqd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gfbhqtvld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzodpgfxo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gvaadrhub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbigxjwhc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gaxqinajy.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gnzmhzjlb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gceanieee.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gzwaymvob.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gihgxljkj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gmnsajzqy.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gczbbzxsq.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ggmjfspco.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gwkkzidrd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/ggzilembu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gfdlrgwfn.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwcihtzsv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gxxkjotpi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/ggghcxhcf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gqwdmvrny.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gvetyiuzi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gtaizvgoe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gmpaktgxu.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/ghxjelfil.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/godlmlgpf.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gyjqscqpo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gujtvnpek.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gmammshnq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gsdolsdzt.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gkmeqdgek.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/glcgxxvdk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gfmqqpeco.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gtblbpkkx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/ghynzcqus.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/ghhcxhrxl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfezkirtg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghqqpmkmk.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gnvjrrcgq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbzxpkbdp.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grdteyndj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gchsrqpzb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gssmyucye.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gpzirjgcd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/godlyfwfq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gmvasphlx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gmdaznnis.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/grttnubsy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gcadvnxhj.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gtvokvhri.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gansfoivd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gvzbtjept.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gdcmffeqr.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gundglwmp.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gsqhvrvpw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjpwecaoz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gnnmoxgze.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gbifgtqug.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/goqnennlc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gpiqzoeto.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gevuizawn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/glydzmvgt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/grwkemmca.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnfzdjfaq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gfhvfddme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gkpaklnsr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ggsplmbfd.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gikpaptly.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gyuodulng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gzujcwity.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gagqiztaw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gzwyqysiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gbtbszgza.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/giczfdjyh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gbatzuamd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gmksdwzgg.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gpcljsnyr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gipvyscuu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gcamhbwrp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjzzsghpi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gqnaaqean.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gfmravixi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/guimdtldl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwqtemorb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ggotimvtj.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gpxztbglh.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gxiklnjko.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/grcvdoucg.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/giftfcemy.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gebeabgwb.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gbypmgqdb.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gitvfbqhi.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gazkcviyx.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gumgubhet.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gdepjtdbz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbxmozsrn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/glafrbcjn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdeoepzic.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwiljnnln.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gdurfjban.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gljjsrzdb.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gtwyjlmbi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gkurednsk.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gqaahkpkh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbrrrscrs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/glgyxodnz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gdthszgcu.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gmajfryxz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/ghirbwknx.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ggodjhulq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gkzihqzdw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gekcvterw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gaunbtobf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gpftosamm.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gcxyqdbrx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/glypqwmll.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/girahaxqb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gafolfvok.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gswnlopjo.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gdprhxitw.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gupvssrra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gywfrvemk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gqynmbtdy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ghdljaggo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gskbnqthk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gdizwyhms.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ggnoombtc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gfjhrupof.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gdhpevmwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gcvbhhjne.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtkfmof.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gfufwmsei.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gkwgvuwnp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gavlbapiq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gxmbqvxns.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gmpucrfzp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gelhovysu.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtngcimvl.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gpbmzohaf.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gjkxfwhkd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gzwcvxbni.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gquzmxetq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gckblmryw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gmexmcqgq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gwtvnrcqk.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnkjemwun.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gtjwaltvx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gxthlyjwx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gjxwykact.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/glqcmuyvf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/ggoipimrz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/grlfuaxmh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gsninibvn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gzymzfgzl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gpsdurdtl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gpuqqgrjf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjpajnvxg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gkahsgvzv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gtgfspatc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/grvtqaryq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gbjwvyoro.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gnjfvpqge.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gxlodcpkt.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gkfqwojoz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gghbgiwhe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gzhjbeuno.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gfyhljofd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gcetpmrwy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/goipkakie.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqhixsuep.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/genfklswj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gpgdnpthq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gmwlqztwx.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gcqgwedcf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grlldrxjl.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gtrkurqpq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gemliegvf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtvbkzeto.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gxbsgnlza.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gsbqrpdfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gkeyewgad.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gifgckuay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gamyljjxv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gijjwarry.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gfdotzwll.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gfnkiqzqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gsjuootng.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaqvjzoum.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfopinr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gopkeghaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gtdezktyo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/ghnuamhts.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gyihzlfhd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gkirclovk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gwlrvwzib.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/geknfovtg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/ghyqhoweo.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gjjybaesp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gchywmpas.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gnceuvaux.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/glxhstfxg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gpslhurra.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gbndttmao.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gxxeeylak.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gitgcvlmv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gdkrwasne.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmyiviht.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gcmdtiuoh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gjwawocpd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gumekkite.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gzrmpbewi.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gwybntslx.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gqsffwmrd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gqactdzqn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpqvyewlx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/giqmnvlnr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gnvhhmkax.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gukenvubq.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gmwlcmldm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/griwmwzob.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gbhyokurg.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gpphjkuvt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gfgbnaiyw.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqjhxeeol.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gytptctky.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhgzfba.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsjenfjgp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gsxhwwife.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gcuttutvt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gixfkyfct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpxowrede.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gyvwlgvcy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gdjelwjhy.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gmljybiji.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gsjfvanex.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjojebnes.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtfbhxqnp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtcpzsptc.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gvpfcsvsi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giskceunk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/grayqolsr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyjyjzkob.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gawgjgfhc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gqxxehqdz.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gtqfnqbpz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gbjtsqnih.sHtML


<!-- 参考信息 -->