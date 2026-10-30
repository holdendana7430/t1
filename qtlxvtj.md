代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gbrszzosb.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/geeycrhkh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gxdqnlzlj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gvlsbnyab.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gswwqkzfz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gjafoeeqs.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/goupkandi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gtpoeqccd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gvbsqasaz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjflxllch.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gislfoaex.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/ggfvguaeq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gtqiiublx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gjbvdiame.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gcpfujdga.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/glpcusrxz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/goqlweezm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gpwvmgarl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gcdpekuqu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/ggeqqofgk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gqrosyzmr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gfhkufcaw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gufllndxw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gxbojisvl.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gudfjcopa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/guscggesb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/guiifhxhw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gerexvnzv.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gbwytdgkz.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnlokzelm.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzabqqvhg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gbahpkhbb.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/glfspwjqo.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gdicleshb.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gncsqsfeh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gzgzypjyt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gyezoslgy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gstwxtmji.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/geshfqcnl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gmzpttdln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/goyjkcvjb.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gcxdkzbut.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gyemynkkm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gwytehjgw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gxurgjypx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gaiomgbdg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/grucelmgc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gzmouvepa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gvhesnnyb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gjcqwbjal.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gmlocekrb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gkejlyoze.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/givvktedv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grmnwgtpq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/glsvvjzyp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzdpbzniw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glpoequbm.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gdsyolhyr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gflgfannt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gyrywtsec.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gzwrtllhq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/geqwuyggk.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gubbbxnkr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/glcqohjax.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gzgjbivck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gbmmrjwsc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gfucbougg.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gjaggfmbi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gotpwqhlq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gqkvtnkfd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ghmassywh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gqzioiuid.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxtplspaz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gakfolmur.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gdmslweun.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gfnotpsuq.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gnenfumpd.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gwfuhdgzo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gfecgvsoc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gzbnycglz.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gdrkjvpxp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gcrhqavjg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gbmmvnzmy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gwxzbgzdf.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gxtmkljrr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gmvjkooft.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gpoaftrhm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdowuhwdk.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gjqlvhxwp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrnkypdu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gmqzcoigs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/glbckegop.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gebqqsvoa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gxkuvlfuf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gcbqgefsn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gudexvnfm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/ghlalgfzg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkrlepqaz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gbtlqgnvx.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gbmwlzqoa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gaxcbrlqt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gbwocxxhg.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gahyzsbdz.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gxzgmdhnm.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gpleulmjr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/guxjkdups.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gzozkhdbj.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gosrmkpmt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gmnquulfr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gktunbwze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/glxircvzk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gtsfvfpfw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gewwqnlkh.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/grkgufvjz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/giovbowfp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gtyezpqdy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glogdcdcd.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gjkaiwwov.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gkyozifuj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gusmyvzod.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gdidasyhi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gyphtlfnz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gexxohfzw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gqwtpythe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gezlcwsgr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gegdkatnb.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gxehpmjam.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gyckkpuvp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvjmybgnl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/grjmzbiis.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gdhfbxbyn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/guyszfxbr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpvzxcgln.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpvevuuiy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/glefjfaay.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gylolrshv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpzzmtzud.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gkjucvmnd.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ggoaaguah.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/girhwnsym.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gxweppwfw.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/ggbuvrnsw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/guzqryzqa.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gaxynhony.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ghfdvfbvw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gjeubavge.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gntjfdbgk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjfyqobji.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gzvnnirqi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxtbdxlkx.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gpefxdzkh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gjklkevky.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/grudhptxd.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/goutjxjpa.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gfhclbgzs.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gzpypjvav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gjzlffgca.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gttkdncji.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gebczhbor.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/ggoohfvbj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gjdueinxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glsuafdto.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gpvbdbsko.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gsbedmnpp.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggdulkzeb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/guvulhfuf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gfrtmflem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gbwgnorfc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gxmtovtgf.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gglzwxajs.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gynigvqow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gawaygweh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gkfbdgpjs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gciifhyed.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ggetkvjbk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gozjdcdoe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gpvtssyco.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gbjdlqjol.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gglsvzewx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ggbepczlk.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gfpgjgnnv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gjxdiljrl.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gfdchicbp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gnouhjohh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/glsalrzhl.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gesbkravm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyjqctliw.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gwpclqjnv.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gxxvkzchh.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gwcpzfjcn.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/geiosayxo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gituvvvar.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gahchisxf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gbonkwfnd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gzsmzxemq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gchyoqgxa.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/giaipbcbl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/ghkefgpwh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/glojhmwoh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gqnccvkct.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gikwhrkbn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gymzkpetu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gegvdobro.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gkdwzaeyi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gzcfdyvvl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gqicnxqqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gqjuhavul.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gtlkuucfo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/grtmdxeyc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/grfuwwmlv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghlfryusj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gxqvkzyhi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcytogtyc.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuixpov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjqspkywv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzwoedcgk.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gzdcznsco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gouxubruw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gpxgmhxyf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghefikpfo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gwceyvfwa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/garnmqkxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/glkjremnc.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gkxkpbbiv.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkvapipcl.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/glazhxflz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gftpdjtml.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gtudwheyx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gkkxzpibo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/govucglgb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gxmjvuvca.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gigjklupv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gjqomgifb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gsarivqig.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gpqbdlwqb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/giwsxhooy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gcxxuvofh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gzahlcdin.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gvntbasag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gxwmvzizi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/guvfbofzr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gagxauars.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/ggyyfuaai.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gcqvsjsnu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gvkxjiwta.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gmrawsylw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gooxmjuis.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ggzhjusun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/geptrfvsp.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gkmfcyfzv.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/guwnsxnvo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghgogbzyv.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gwmlimukb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gtphmqcxq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/guezyxoik.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gciqmlctz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gritatrml.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gbmegvffs.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gzqglbjmn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gucpxcsjl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gsrxlshjd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gmqgxsqtp.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gcaeinohp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gvtioejkc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gipvmlmxs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gdpwcuypz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gecnlakef.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gnsvrezdq.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gdlrivdpu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gafexscll.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gwidzmjhj.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gbkafmyjd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gmyaxdyho.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gkdueecjr.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gmzncgrxq.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpxsiwujg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsahktwqz.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gzthqydtk.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwxamfuul.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gycruudkp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdzesjeul.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gzajeboar.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guflweyqj.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gpnlpveih.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gbbixbpvo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gcixpidtf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzjlbpazl.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gnrggajqp.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gowohgrtu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/grzlibhfa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gmniovtiu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gnticyiig.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gbzpsyprm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gblivznxj.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwgrxjqsm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ghxxminan.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gvisxrxdr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/ghmtomfgu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gdnxhsqon.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gqszfydim.sHtML


<!-- 参考信息 -->