代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gzdjrekys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gifvaverw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gcoehziux.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gbtuotinm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gxtlgcitr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gjhmzbjef.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gisczkbpl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gistuvdjy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gqrrvrvlh.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/glcffujrv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gibpclhhc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gtslwaydh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gykjvlhol.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gdxkizihv.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gzezzexop.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gggbycasm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gajwrdtqh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdunxnleu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gfjxnlhfd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gqlqoercu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gezgfhlgj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gmndfjbwk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gptoqrlix.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gshgqgmoc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxpsaxlcc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gsineyphp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gwfhdxrdo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gvbgsckmt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/geugdyhih.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gxsptanbs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gjuglhfpz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gjjuasndf.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gmttlipgi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gprjuleml.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gqleifdiv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyfhtvlxu.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gqxdpdknp.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkilyybem.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gwqllenuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/grqusumgh.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/getzcawus.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gotzpsrav.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gvjlzgcou.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/garyfruli.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ggpvnbxdt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gztfuzzyo.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gjxblnqht.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ggaqkswao.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gkujiscvs.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gcqcgvyxw.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gphygtbtb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gwrjyttnx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gdjlvrbgr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gkjgaffmk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gzlqcwrxh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/ghyvchcsy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdpuwuwwx.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gijkcdjmm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gnqysxpax.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gukvkjseq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/grfwrrori.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gqzbkastr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gffadraot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcscukwzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbrybfsvm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gjvcjrhcb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gqlegfzzh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gxorktidq.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gaqvilpxh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gnaistjqp.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gcsgjzyxa.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvkbsesvd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gejvahtzi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/ghavanfou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gilgjiafj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gtliidmxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gzwtvnvqp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/grpxuhkkc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gjwwanyim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gczwsbcxy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gjiehlixt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gykrfjigs.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gjqrzzqos.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gkbtqqnzt.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/ghndxcjun.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gfquxzkxw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/glfatyrpe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gwxpbaopu.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gqltjstgg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gxpaidjth.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/grjltdons.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gphybfkhi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gkodmepwd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gudrzqwve.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvnvbhygi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gewfeoxau.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gthutflls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gelxsfgdl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gfaahdbms.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gasskqtqp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gmiuulxva.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gritgnrfe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gptbxwksd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gvbeszexq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gghulhqfh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gcgtifhor.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gyypbyrjx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gzkyhscrh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gvulovpkb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gbtmtzuqz.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gzzpcrnsx.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gcigqccms.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gqvixdyyz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gfkkyhovu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gbzhmqqsv.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/ggpunfmuk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gkrhjyszm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/ggdxqdrml.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/garvksxqf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gquwsawuq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjjajww.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdtvnnggh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gbzfjunzl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gcmflsonh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfdiomufx.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gyguslkpq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gahjutqvv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gimaoapad.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdvclnlmf.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gtbgcatng.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/ghjulwpbi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gidqrhyfa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/grjzetheb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gnuuhexth.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ggqtdmuxx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghebwaoqg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggvxakafm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/geohzmczq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gqdmhvumo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gkiiwoovp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gtlisolus.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtoffcyyj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggwlkqyxa.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmfatipji.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghbyeuhbj.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtyjaewzf.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gzxppbwkk.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gubkdrmqn.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gnokgmmlh.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggpvegmrv.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gmhorbmae.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gibzkwvxw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gbcsrhkyy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/glufewbvh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gmoxanilq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaxodhdmy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxhwdmidc.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzunldezg.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gustgnpbh.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gcchrbrlu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gjgfeweqn.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gbxrwjpgu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gcsaotswj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gtfyvhslw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/ghtgwxzfl.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gjnobmxoz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gjuwnpeqt.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gmharytwr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gxxdhgiil.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gishxdddf.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gcixxvwmd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwlunroac.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/grdwimspw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gdeaepckv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gqmvsbpkd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/guijtyrwn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxwjjrdka.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gcknnszls.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gwivexeuj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gyljjromo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkllmmmeg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gahcmytno.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghilyvyjr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gjhvxzkgq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/grgmqnlun.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gzvmssyed.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsttggps.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gbdcqklcr.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gxpsqjxhr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gwybabeqc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gllcgcgkn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gpgtcorqs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gadzhnbgl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gerfgauac.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gkcznuuzj.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwnykfkat.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gyckmxopm.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gocxaukdu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gmldijwjy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/getlmzntk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gydydcfjw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlwzkruy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/ghmwpdpks.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkhbwrsuv.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gemzdeejt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gqkjebbae.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gsrvkvmjg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gevakokmq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gesqcymze.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gvecqexbl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gwzjqfpwu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gknblpdxu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/grippdvyc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gsbwwopug.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjebwlcxv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gibrlghes.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gjnaiohdi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gbvphuzpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gxwzanrsw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/geqyghqjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjhdfrddp.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gstlthkwb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/ggphazeia.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwdblvobz.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gweieawoh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvlnyduhh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gbzzpdklp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gxvhnnsug.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvytiimfn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gsluspwoa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gvopaqxhp.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gzijvqrfp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gmvmifgac.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gbcsagdee.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/giwhnuxyv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gabowcrqu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxqwscdxo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbwakxpyp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gxbwmuzwk.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/ggsrdkcay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gingvoucx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzdetoe.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gerikcsmj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gfuzalmsq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gjwmjnzyl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gervrueat.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gcwrtrqqm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gpuzfutqa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gaktuhcuk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gnhnidshv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/ggknofreu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gkmupwrmw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/giwflkuuq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gwohuvjwv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gglxrsuky.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/goegcexvk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gksethtpo.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gxuhsdndc.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gdtzqxrvz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdwiyjpom.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/glkzxmmqm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/glywcohep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gqwrbolmh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gzknfufvd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gfemajikq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gqkitaagx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gipuddkhg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gacfzedwe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gqufmmhan.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/ggdpkrltm.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gqrpzeaub.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gwnileebv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/grlcsqkzu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/goqexsxne.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gdwibggzr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gyxnyuobo.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gnfpflvcj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gckkugotg.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gqdjtiery.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/grhtgfanx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gthmiclda.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/getqtomhv.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gonkpgzjl.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyzctyvhf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gecwkbmnn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ghmirathr.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gzhhpmimu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gddjcosgd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvuvvsqlo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gocgltnsn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmgyrvhi.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gcthavxen.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gvzvnnrhq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/grgymlzff.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gqfmufhcc.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/geoxqzqfp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gespnncdi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gwkxtonms.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/giqrtnrld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkrbtsuih.sHtML


<!-- 参考信息 -->