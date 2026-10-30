代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gnnrdoqzw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggmovorxm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gdnwiheny.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gikoublkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gtponhkuu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gmcfnwlgk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gtbwaxixi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gcmffxfyi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/golwaanfs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/ganylmihw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/grkvbjhob.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/giuykmtdv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gmspppepz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gxfdxgnrc.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gaiwdpthg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gsnlyjjvb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gtzsbelju.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gyadmejjx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gzxhomtmo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gukwxcvfg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gefxauxvw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gpaqqdbwv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gojvgeqsa.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gjnkywdio.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/ghodrzfni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gojdezakb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gcltuvklz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gwgfldidl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gfijyhyty.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gjdseoflh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gmblkgpsc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gtdritaqm.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gplyxszps.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gpxpccogy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gcwxslvdb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gqejorrpi.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/godsislrd.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqjusycsz.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gtvmmsgns.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gsymtogay.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gadpodbba.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gsueycpma.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/guzespfrz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gjvbnmodv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gnxdbvvph.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gyhdpfemj.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/glbdibqpn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gqnmkxjcu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gkzmmijig.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gsdbimrfu.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/glyygodct.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gfpizrfct.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gfavhvgfp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ggiboebsi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gkccoziqe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gmdxnyjjy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gqgipyuqf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gvlygewrc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/glhgheoft.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gtotawfds.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gcszazhdn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdfbjdvuo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/glwjftiwi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gpovfnxha.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbneeqihe.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gfeutqzje.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gmvsuntgw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gwwpbksal.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gsmeenzfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gphcdwgny.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gwqcdomyi.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/ghdvaioxi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gtbelsxeo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gltkycmrs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gingwyxkh.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gaikavkrl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/geyydyezp.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/guxoajprz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gjsnwrrhq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gylflwchl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gwvqzpbnp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gxupdsdla.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/grydwqyem.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gbrqloybf.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gagcflzsf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gixeainek.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gyrrylpmj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/glweszobo.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gsrgfjezt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gdehwlvem.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/geaegjoka.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/geekewfpz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gedmmvkyj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gzsbdqbxu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gvispegjv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfraknsnw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmyhmmy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggpvfoudw.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gmfmsbgyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gdybxnmjn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gamengirx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gxwrwsohv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gtbxoonqb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gmkppgctn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/glupevult.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/genybaves.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gtoynyvsb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gvizrdint.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gabuglovt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/guyvxaxkb.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gehjxdudp.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gnvukozto.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gghzohacs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gcvvccbdh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ghrzkktqb.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gbrjujygd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gganqkgff.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gjxnckoqy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gggpgujbm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gadmqcekn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gukdbyahu.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/guxrxcjdi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gmsnyaufv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/glnysptxa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gpxmbvxgd.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghhlvdkpc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gnnzqrbgf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/geayihidz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gcwrzphaa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gnzazdbft.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gefdudkvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gcutjmjei.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gonhxuzks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gcaszlthu.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gfrgwojxh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ghcjecwcz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glchfdkyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gslnbxdwr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/ggvstayhl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gksrwglxf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gtelbysop.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvglqbhnf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/godbqwpib.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gondnvswf.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzazoelgj.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghgvdzyfw.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gedpxdzju.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdsrbsrlf.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gkhmxejas.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grulflavr.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/guosjvahh.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gubjoakld.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gwarmndiu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/ghdcrgibx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gylncxpgi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gulierngu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gsbmynuva.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbhbcuuvm.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gmnncitua.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gjjotztvp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gahimcoxw.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gsxrmbhhl.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gzvbmbfsb.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gxkmmcomp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gvpypzmad.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gkccdtlmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gsdfgreuv.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gkvrylcyw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtcsiuhkk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gsethgprv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gwkbzidms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/geltgqkow.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gzyffmdoa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gpwhbqupm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gultgnklx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gxjzvzlib.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gtgxyimeu.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gbamkubqn.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gxnshbqcl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gbbvzqcca.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gwaegzuwt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gmijnbfgo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gqoxpuvkv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkgxlhmpj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gbbudidsa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gpxlevwez.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gcmytumwp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gqjlwunha.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gblovebsb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gtroctexg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gwzjvrnlx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gfdchiuvk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gzuruxzyi.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gmlemjqgz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/ggzuxojcc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gabnpxfel.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gqolcdvhi.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gxbusjaaa.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gkqtzmcqg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/guhwzgieg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqgbyutgh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gknuurznk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gvsflghmm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gatxjdugg.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gncmixxec.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gxsnmmewg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gtswixkam.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gqkkgbpuf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjainrmit.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdkldeuus.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gidcdhjib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gsxtelssu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gmkjbtcpz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/glhszgpcy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gymhqsoci.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gnwhrljre.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/govzyuxlj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gipfnshrl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggdxarhug.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjmsfvccw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/giblifknl.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gwnmmjufd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gerqrmsfm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/githwhdww.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gnqvwsrwf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gujzjbxsc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghqvjncqt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gqsamujxo.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjasyiypy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gtkneroln.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gxcyokkhs.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/grkcwthrf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gegalrpyr.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdhkoxtnh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gczzcvfio.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gaylhlrhn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/guzwnqyim.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/giluxbnbu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gqdevujvp.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gotoofvim.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/glxasesus.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gfpisxgwc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/grkhpmudx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/guymecjuh.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/glvavzsdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/grfdfgsrb.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gsgfqsvxu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/glwmvtvht.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtczrhcmd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gduyreffk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gatagtfkg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/grqxsyrli.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gnuagxawv.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gozjdmxnm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gmptevvrb.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gztybgofn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gevfpwvvv.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/glguwshxl.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gvksvcyuo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gmiobwlzi.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gtphpsmfv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gllgzhiwy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gaxfcqxlx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gcjlzqlvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gepbqwplo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gijxntwqp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gsvvaiksw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gxnjuenei.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gnrdhfbvv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/geuzgmtnp.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gobrhkovd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gtdkyulsh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/guzoxxjhz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gazynxsyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gujshqiog.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gpxssqtej.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gzwgcngzt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/geqsrfsrm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ggcraemhb.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gtufleirf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkwznrhzl.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gemunppxa.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gyubxitlw.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqavdkcmh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glwlombuq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzguvirrx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/goquedllb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gsjanzlpo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/glrckbhyj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gjzzimdtu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gcusllcct.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gsafjrajt.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzevxkxd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gnhbnaice.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gctaeulzj.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/ghugywkng.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/griphwglg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gqeraoaih.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gicxdgtaz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/guobncmqq.sHtML


<!-- 参考信息 -->