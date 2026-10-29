代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkamksjvn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gwqnkaqlo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gkzrvnqoj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gjxhwrpxy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gzibqheeq.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/grbzhpnkw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gycxarreg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gxgrwslbh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gwsjnznpx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gdsptjbfz.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/grdoecqvy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gfhfooolq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfdjddlb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvhnfvc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gaaujwmkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gonkrgfol.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gpdwxcnef.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gryjuoqfh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/glhdzeida.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gezmrlbrl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gdyorlvrt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gkmfmiokn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqegsaghh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gjbifgekm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtieotirj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gqggulanu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gerylzhmm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gwkmmoajk.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gvjpxajxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gfkfjcowx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gezxfgbvk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gsvtkvmje.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gfyguaqdq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtbedhezl.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmfkojwmy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gnasnpvox.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gakygtjua.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gatwblnlt.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gqcutozwx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/guiaioeck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gmfeuqxxh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gctemwchx.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gljatmcci.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gvgkbctez.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gqulhqqyk.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gylxzvcpz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gskpofpuc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gaiiglfqj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gozudfvwr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ghunblcis.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpktensqk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gvpzglbll.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gkskyppqx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gvcfnrdxb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjxmqtvfh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gjwkizqfp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxptcuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdzshiibl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gftdtoaqj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjrdiucop.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guovwbudz.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gpipzcnqy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gaolvnizh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gxvolhgxg.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gqmpzgysi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gdlkqwtcs.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtgmmambd.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gqpvnueiv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gxzezahrq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gbyrpdxyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gojwmbguj.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/giwqyoakm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gvffcpghg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gbtjyjlne.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gdpvqhfvw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gfxdcyuqb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gufjvjako.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gouvzltrz.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gxrfwgyxo.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gyycqestb.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/giplrnsmr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gjttjclot.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/grhblesxd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gkceggcma.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/ghdhwcoui.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gtiypbeno.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gtxnpaolu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gmokmqgdm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gzyuyxwdp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/glnxfvfhl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gkchuxwao.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsvrftixh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gaahekxtq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfbycxhie.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gerotwcwi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/guyfcvjpu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gplmobrik.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/grfmzssmn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/grxpwybgw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gxtexqyiz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gccycibsd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gtorqkrhm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gdxlgttpg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gaddlnxai.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/grwhyjbhe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhloerhc.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gbnclnpup.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/graqnvshq.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gdqyeeidl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gqcfnvuib.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ghvdxkodo.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gurobfdka.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/guoakxpvv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gevhpqpcn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gihogtltl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/giwmklcwh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqsvuzal.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbqpiaewe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gonzecgpk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gftszscnn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gqzmotihz.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gswwvdges.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gyubyjqko.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gxhfofijk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gnyhhxfoj.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/ggbbszfdt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gxngkdoyq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gugodaotf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gspztbnmf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gqpwowlfu.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gfthdgzue.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gvbsoodpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzkdqdlks.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gayvdxdmr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gqzdrspnh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/guycqdhuq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gtkgyxwxw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzepyoimx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grgatarmy.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/guczyxzso.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gbgdatzma.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gjbbrqfww.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtmumbkky.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gwiprzlip.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/glztsffer.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gygwkvngn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/ggybuusbw.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gdugqaynk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gmidnblqa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gylqkhtbu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/golfdgvpw.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvlfbgqok.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gdsoexrzg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxfastmsc.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gvxrfaugd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gvswsmski.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqzihptso.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gpzujpnfn.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gzgyipeug.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gpahfzhec.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/goavztcoi.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/grrxdbvmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gygxhectc.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gqhktgsax.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gltmvyqvp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gudybfuna.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gihyhhjfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvtkstnvs.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gjbumcvxc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gbnjiaugw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gqjfzxmix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gwjdjbfsj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gbcbsgiwk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gzchiisdc.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gzgqubeod.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gdxngfprc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gjeazjapa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gpuciiqel.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/guzrloawh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/godbnfzyl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gzhyrnaqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gpyvqonzm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gpeaunwpf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gmtglecqz.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/goosnriyn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gghqsubtz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gtuspvbvc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/geddsxijf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gyasykqaf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gajdypbey.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gcvyizshj.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ggvuyhxkg.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gmcfltyns.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/ggxmfbknq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gtnoeaoyi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gltbjbsfh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gubdawnrk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ghzaxmege.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gjhsisgvz.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwshnuofu.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gknlammwx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gkkausoug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/ghelddyzw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzxselcas.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwxbtzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gmnmjpbwg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gvlkctyev.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gevlysvek.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gihurzeqt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gyypjmkpz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfyknsjki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gjjvxwxck.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjggnsykt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gcudqbdsq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gligpqszk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gnxpsexja.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gjnjlfwju.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gmsakuzdu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/ghpbamxio.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjhzvvycw.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzbhcqntd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gypinqxtp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gzvgnarcw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/glbzxpxkf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gqejihydt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gupctciyv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gcnwohsxq.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gcqozfmxq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbbkzjlff.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gxmtozseu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gntxsvocl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gyvugknpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzgvtnogt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/grlmtjcyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gmazlsxio.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqsexoksj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gjpnzfnvx.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gyehzvhbj.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gmpoitimt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gyryzsbbp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvoyotzh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gpmspwboq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/getqtpbqg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/goudpdjyo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/glfvuciok.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gqsmexguw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gljrjuuhj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gkbubsvte.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gpxpyewso.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/ggugsxmmo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gkeyrbexy.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gdattoeve.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gnbfqnhnf.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/glgoeoybx.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gzzaxzaxb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gltakcict.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gaqlmcpli.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gwlvhmdyq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/giipetvvt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gumuqbnkq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gmsrcskuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gndmzqywh.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gtazittnp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gwdwvmutx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gjtpzyvwk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gnbbxnyrf.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gvlngdjho.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gdxlbzqwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gpxdgcuog.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/grblzqmsl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gexmqksqr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/glbrmfxvv.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/ggmcrekps.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gxdatmlzn.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/getsmazhf.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gudhvhzhm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gprdktlvd.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggcdfgpmk.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gdewjmvxr.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gkgjwiwgz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwwrjvwjc.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gfxcxjbnq.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvmqjrmkj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gamhgyjvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gwjtddxti.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gkngilfyc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/glpobzomo.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gdmixbzqj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/ghxjztsxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gnejehwec.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gdsegtaqd.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gxfasjpow.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gvoeczotr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gbiwkutqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gjlkztuvi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gwcaqwpha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcppcnymu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gwfgykocr.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxgznghfb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gegirshar.sHtML


<!-- 参考信息 -->