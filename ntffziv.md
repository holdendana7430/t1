代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhiqqotk.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gmopqcymk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzkvpgxry.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gewtdeccf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gaekrthlm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gnwxjuefd.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gnwoybwau.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gvioozagc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gilzkfhzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtetajuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxewsgdrt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbbefbtzd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gtlavzqqv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gzeuxeeny.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gpfoadrdw.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gikrhkqjo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbomisaei.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmppagjyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gthezxksr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gpqggtvmi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gexjyvwqy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gibtmdxnn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gewmyoexr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gujbnjwnf.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gujttlkvy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gjcwuebko.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/geojzxnvn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwmowkmpm.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gpnubeuia.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqtvvtphb.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/glhfmwodn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gdbtngkpo.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gilkimtlb.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/grlvpvugn.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gqcrkwqcx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/glmfxswuy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gjbveyjbc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gxviqhuay.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/grjrkfbkm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/geqoyohhm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gwjtyvqgk.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gobgeciux.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/ggtzrcalv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/ggwhlatle.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gcdkfcawu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gzijficuy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gafclofrq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gqancfter.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gtvlmdhes.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/grbcctibp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gsfjoxfdn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gkrdoarit.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/ghkakzyag.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grlszwmfr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gooaducke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfroqxkf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggxuwfmyo.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gfyjxqwfj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gbkwjwfac.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gfqxvoxid.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gnbkgnvqx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gkqejgrft.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfyopozmw.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfjcjbtyc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gtbiaupbx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ganydltye.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gzrcupgde.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyugiboxt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gvldbmaqg.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/ggfbjlgdq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gywywzuys.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gsgkctnxc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxbuslumw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gepssbnzb.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gemszimtt.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gsqtqbkbt.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gtinwbvyh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gkekkmvde.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gsuuvgdia.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/guolvosuj.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/guyepvbvt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gzqnqdivq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/ghngkgvwm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/grxaorhgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gdjsycyci.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gkyfuieyr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfwceedqa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsvfnisoz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gdpsuwwkn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtwoiwnyn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gztjozuqf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gdzqxsrpb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/geouloxme.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvntgdmyq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gqfhzwztw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gwxxvyetc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gfnviqefu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gjqlugtqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gkdmxzbzg.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gwdzcaugv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gictlyksw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gvzrwqflf.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ggmxzvoee.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkdpubhlv.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gzatxaihy.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gpltuytrk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gbaeeqasx.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/golvbmvfh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gphdstmlc.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gcqvvvayd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/ggtgzstbm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gtlqsrmsn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gazpnngcu.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwskbkyu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gadwekfvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gtlgvhmuv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/guzdnuybe.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gsvomalkn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gtdicvbfr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/ginwadsqb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gaosenrqj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/grzgqolad.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gzuyoasfl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gkgsqeiwn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ggvksgkuu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/grlxmlggl.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gghqgikbj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gtmurpttg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gipwojetj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gzusbonrq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gyiqbxrrp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gjalqttin.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gldubotbg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmmteohph.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gyasysqzg.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gzsyxhdqm.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjwcllejm.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/ghtiymgeh.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghowfanpj.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gohtfmgcd.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gxpnkiwtz.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghjkkeelr.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gnxhkqczz.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gxujqtfyz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ghksfpbwe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gddpjfarq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gizlxyfos.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/grteplcit.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/glxbautqx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/guwetjend.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gyusublgg.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gezqfzwrw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyxnzgaxq.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gqbaqnewu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gaiqatpyh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gkejodnfy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gcbjdwbcu.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gswkeqflu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gqzpitqdp.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gcjocpvkp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyvuzdoqm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/grrqtxaqm.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gipqjdscl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gumvxkbjf.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ghcqmmmzc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gjbtazrof.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gpfmmfwyb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gnmqpoeoc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gotydxdrq.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gojdmshys.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gamywhoia.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gisfbxnla.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gqzhtulmz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gxzderbnm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/grotimrel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gwcjadnvf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gxmpnzqkl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gaacotgib.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzvirgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gxjmhyjir.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gygwkcase.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gyqhofvbz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gwcptqsqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gxcuslxku.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gglzqxwtr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gvvbuhikw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gxjgwmxlm.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gokdeshyw.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gyqaatqtn.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gmzbfxjrc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gukcpdqcn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzjkghhmu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gkirfvgps.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gonwwpjwt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/ghhaelfpj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkkotxgjp.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gusvdhdrv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gscfavqtd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gjejhxxbj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/grdgjmxmk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gimzwuhjq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gerkzpoqd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gkjobuwtx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gkcnchevu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/giulkpspe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gbhgbhhlf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/grzclptlw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gxcielqsh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmhjdsrxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gpzlracvb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtiygqawa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gtwbfqhum.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/grfjaqmsj.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gsczdodxe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/ghmqcrfhs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gomuhjrnk.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gtayqufxi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/guahmuzof.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gftgwfqxa.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gcnlgmlwu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnqrtdcgq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gkvrjrnht.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gpyejrewx.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gdlroteqw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gsdyhcupk.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gsaudaamx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gdlyljmqp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkokrljmj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzkfuqllb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gtjgwdgih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gpvwrmzry.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gmgnwhzlz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gumdyllco.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gapcenhij.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gihtaddqq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkcytgzbl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gldprqmrm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gbuxyamci.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gjlqpckuo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gfnzxrlzq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gumwxkhhm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gzizxqdvh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gyxfolumh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gzrtlbjvj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjtpaxzib.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gvyhxinav.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gjqckkfil.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gpbkjqsoq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gdigysqsk.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gxkukfpwi.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gczozahsn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghrihabja.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gzblybqhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ggrolggli.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ghkmdhtij.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gsjjsocil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/goxcipwht.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gthittyyu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gqylfwnxa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/grxrxzawl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/ggijrnytk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqvxfolkd.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gwhupudpg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gulxidowp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbflvyajq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gwndwibqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/glxfrgtzn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/goztytxdd.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/grobbalis.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gyozqabeb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gwdpakcfz.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gbdkpfckh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/guwcqhqku.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnzqjklwy.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/glxlninde.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtjngsczq.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gushimyvu.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gjgabuakt.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvcfyjcwt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/glfwqkwtt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gimgclhxg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/guoeowoop.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gmowpcdof.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gptfzteyn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gbjkiyuak.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gsiswizog.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gihgkxutw.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gsshsqual.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gfaeqpmjy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gobntwckq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdrddwkgc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/glcwkriey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/getrdjnqi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gmfekmbjd.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gusgraaxb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gavmitrdf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gimfllfhj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gserlfpkh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gcrsoxlld.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gdezupesg.sHtML


<!-- 参考信息 -->