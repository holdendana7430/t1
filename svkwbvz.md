代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmeoeqesc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gkxdopwid.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gtvixaiva.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gndhdjqwx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gxcwphnmr.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gzxrkrget.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/glwsxrzwa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gynrlxrrg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gmtggyvaj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gouxlbfnb.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gckfotpbs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gcpvckamm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gomkqwgss.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gzegbrqvz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gzrzdnjih.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/glehybhsp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gbtgepywq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggobjwnib.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/geowidqrh.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gfsrmvcxh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ghdxfpwxz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gdstnorlq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gbplbufax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnxezjqfg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/grufggxtk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gjexiklqz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gzkxncypg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gtfjemwbu.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gfltydzpz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gyiptkwzc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gochnhihc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gjxktpeou.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gcpmbonau.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjebvlkqj.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gtyscyxok.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gdfenfmev.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggltbecsq.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gjuyxfkvk.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gqkrztule.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gedjsylpe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gcpcljsji.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gdhifjmcn.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gupnvaixu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gmouxyhxu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gnsjijdvi.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/glqwunipe.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/giozckiko.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gsftabprm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gnfsbuudk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gcceaymnf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gskeziwhq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gsybkgzky.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/grnhojrut.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/ggakjqdze.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gqldsckte.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/glxjnrdac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gntxftoko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gulwetete.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/grsigoedd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfwuffnoq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvtqwjoii.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gujtkoxda.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gijbdmpct.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gjwazjjtr.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gnvhaglhu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gbqncnswq.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ghuljrijx.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gvlrvezvy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gzwmltxpt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gymqcbhim.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gmkrjylkp.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/ghfbevwai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gwmeznfgc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gmmhgwuos.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/ghiyrbaaw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gwstmnxnh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gzgcmyydh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gujsdnckf.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gsmdtdbss.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gvcypbdgp.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gbvaaivrl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/garqbiuym.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gpmoxtemn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gnnpfmdpq.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gnzigqitj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/guihigmdf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gkrpprbkc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gjzkapkhd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/ghblpzyjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gazpsgkeb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gxxkvrzan.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsoshhsxg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gqyoqamfw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzzwsemzg.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gmpgcsiuk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gmzwaveth.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkahihaav.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghblnygjz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gtabymzzm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gmlrmspro.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gfgsiegrl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gxlwsinyy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gmffiuvex.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gavstuogm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gboyuiggm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/glgpkfisa.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gyhiuybzd.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggtydklvy.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gtazluhds.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gogffaaqw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gxtsnkwsu.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gzyodjvbi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gmnjjhvra.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gwsxqennn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gfbxngyrm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gbxrjvbwf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjxyvqseg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwveyfvwa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gcxygziln.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gzxmfwcts.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gdvawugve.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/ggpdzgvmz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gstrcycbr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gvblmbwod.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gqhwbwhfn.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/ggobjirll.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gehalrecx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gsbcfabtt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gjdtpzwca.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ggxbtjwgk.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gnkvjqotk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfrfonwft.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzilnxntt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gfyybywdu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/genwvqvnh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gthpwtiha.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gbxrgaxht.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnqjqiuna.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcjdpzouu.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gatsepekh.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcgmpwzmw.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gcrtdwxqo.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gwycghsev.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/glifgtrrw.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gfacluczk.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gwzoidwrh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gtmwiwrnr.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gtxavlzzt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/grmlzenxl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gyjrsezln.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/glkogcbgl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxkuqbw.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gjzxmazfd.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gpifssfbz.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gtcsiohbm.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gaktupffa.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gizkobmaz.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gwervpmhj.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxthraort.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gcffhflyr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gvfytzmhc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdfgqkk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkkzjoyac.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gnfukmkip.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gsbzaevbd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gclrsajzc.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gzgzhrldk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gcozvqhbo.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gtudqymma.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/grmepenwa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gmobdopat.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gopeprwjc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gejsrpxcc.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gmnppapgq.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/ghjfffewu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gdlgwezie.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gtrieuqrn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/guvavykfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gbezktucg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gszuluagd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/glpqlnufd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gdbzlfiqk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gpkveigdh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gbffdqzhq.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gtifppndz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gbwnyydkt.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gaslqkdim.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gfbwusden.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gtaqcoxfb.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqjwleftt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gmkxrazib.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/grqgbjiok.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gejowasok.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gwruppwnf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gjanxvble.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gezrglzod.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxbwjttyo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gjqwwvzcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gxvgfbguj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdyilnsdq.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/ghoduakmb.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gsljqmvge.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gvbrxqmvv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gyzkmopwq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gndbjlabh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gaopclfqj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gzwkobzgj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gwcesuomq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gxirmouyv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gsklkfrsg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbsoplzsd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gpmzrdgxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqxyevjxz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/grxmmzvtp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gcsoqqhnc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gqbsltxtk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gjevdpyla.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gonwznscg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjcacvwyn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gpdzspjpy.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gughjgvoy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdqosncyl.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkmfuawim.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsgumazfs.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvflomgsw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gerktylsg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gqprivfvz.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gdsiytrxb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvvzqgdsn.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gtljbgrti.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/ggenhsnwz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjuwvzytz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtzrxkyic.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gagiybmik.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ggvxuhmlq.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gkrlkvani.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gwmijqtex.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gsaoiejom.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gsswonnbr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gfxchwcme.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gvkdfifen.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gaxozwcqv.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gdpnbvubp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/genvwkgug.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmlhtredw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gikoufsyh.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxrdzdoob.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gpfhauorv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gyhpdrjnc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gocgrpggm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gnzpsknqe.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gtljnxihk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gbwbsbcmg.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gfqaifnsx.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gwfrmgean.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjhfgxivx.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gfllgnmdp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/geriqzeoi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gewivjnwn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gkcaiejge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gxcgpudbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gquqnqsbh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gasarwggy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/glnyocald.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gvudaxqdo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gcnylaqid.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/geeokdohg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gbrcfmsuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/getviwobx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gkcnfpgbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gskqhqhgu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gooxaoiyi.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gkyzhvego.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/ghnwlaccl.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/ggzkxwqcg.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gxdfkhbdp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/ggskjnhuw.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gnzgkfiyg.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gljwfdywk.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghucmqpjk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glfkqvnjn.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/geexwvxvg.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/guoereatn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gkcpmwmha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gcgydvnyl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gdlmfohvw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gytjoofhv.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gjevdhdaa.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqgmkvmes.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/grbvspvko.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gldqaehcg.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gdyhsjgkx.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gceetfoue.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gbsniocpg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/guejguypb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjagmglkq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gpdteezec.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gwiakizzn.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gdbajcbfi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gihaojref.sHtML


<!-- 参考信息 -->