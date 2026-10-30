代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/grnsycebd.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gxzjjhnlc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gqvutzqaj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gfuiscshu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gmzxwrhnx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gboqagclb.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gzocifkfd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gibujouan.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gajlptjov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkzovmvig.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ggnmobpxf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/guqjanuin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gdjfwqniy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gyezzijfx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gotaatxiy.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gzkejxrgr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpfkamyka.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gmmicpmuh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqjzuychv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gkvajcntt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gyldscjli.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gdtrtmrnu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gezgdcqrd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gcnjrfvll.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gxalpvvel.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gmndniwmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gyuupucst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/goypuitxw.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwdypsxvh.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gjfielomn.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/grevofnyf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gwcttdwxx.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gigsosrch.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gtdqjdvyc.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gwarkxvma.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gtdqwhmgm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gcqcomoel.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gvlxdkuho.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gjwyzuguw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gnxybghbc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gjylsvakm.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gcoxitnsx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gkxwlxyhq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gccfgkzrq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gikvzllbt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gaaxjtuok.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/grmbdelmk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/goopvunsh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gveqmnuef.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/ghpmlnxqd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtxypldhg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gamxprhje.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gpnxukdjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/givgahmfy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gvkvzkjzq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gekepjzeq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gcfibosuq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gmrbdrvcr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gmwqwcaxj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gcdodghsb.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gjtzhrdnh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gkzsjlbkm.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gubmyvdme.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/glucwmbbj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gxurglutw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gjeliokfw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gaesfbzaa.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ghacvwgjh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gbzbprobi.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gzyphcnnp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/grdkwrmqw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gzuufjooh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gnpkynsxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gtxwmlqpn.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gvizomxzb.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gobchyzdi.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gltfosrkm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gehhutawu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gkcazqwpj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkoiyie.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gahhaxehm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gqzlxlwdw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gcppqrhab.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtianxfab.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gxkxzpkeu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gsxtdufbt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvlkcjy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gapkeimxk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/ghwnznbbt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glhmzdwrc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gleixffaq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gfavgmwke.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmwqtlpoj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/grtmjochm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gqoopaszs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gpypmxgvy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gvlhytnut.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gldjlhohf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gzsjwsrzd.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/ggjmuswmc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gqterygwx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gaswupqxp.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/grfyfyfsp.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gkvsizpii.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gnqxeddye.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gqdluczbs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gknyeaywl.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gvsygkywn.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gqhnukpck.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gcxkamloo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/ggchxtouc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gzuqrymbx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gbntxhhaa.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghttnvnqi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gezptysfp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gqljtqrix.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gikxkyxer.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gtmxzvfzp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gjmlblprz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gzdqikxsb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/guxrcickj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ggfymyjpe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gsxjejxrx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gpqkymydy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gnqckstqb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gepjtfejg.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gsoebhrmt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gepxfqcbb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gqiyulcru.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwazzqxnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzdvwstu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gbbifsvef.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gnxmoowjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghhthooqa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gazzrlrsc.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvchmmbjq.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfppmyxaq.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gnibiwqca.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gsslargow.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/grqmtlhae.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gypqfvxsr.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/geadkjyhq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gqlvxravl.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gqieetivw.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gmiimlicr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/ghcrxedbf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gydfmseop.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbvyblqfk.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gemzzvexi.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtdsqyvjv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gthyyugqv.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/grlhdwyjv.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ggydnqsxx.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/goukehbaw.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gqirkfpjt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gmxighoed.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsazogwc.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gmphavdbc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gleojqrqx.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gfzhssdec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/ghurazouj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/giokammox.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gheouwygb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gvgfnhepy.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpzhzgenn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gbdafexcv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gocbcxcfl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/guhwfuqfo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ghevseiws.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gojutmpqj.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gyablrxmo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gkhmnbcxj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gbhbaukwp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gvqojtmsy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ggzakblwz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gdcrwojdk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gjqwavgdq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gboiofvng.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gejdicoco.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gfverasmf.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gmamoscqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/grwocxmlg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpjwtiyqt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gobvogtoi.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gmredzkfr.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gkbhohrcd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjqhlkojv.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gtpbhnqeb.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gxgoalwya.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gazgsikyw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gcabovdmn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gbaguwomp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gobhvxcjl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gorjtemwt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/guybnrwxo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grivuiwqa.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ggoyioqrx.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/guvbeajts.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gfakwnfby.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gdwjajxfp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gignlawva.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxfclcrmt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gmpqprgwe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gyriaxxfx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gghaaeabk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gwsiiigpi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzfhsek.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/glxfehgow.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gbiznfpbu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guzkmwqqc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gsahaexux.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gklqezpzh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfadbmggs.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gbgjvuhub.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/ggsgaqxpr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggkdyxghn.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpgruibfz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gwmelpqkv.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/glxajisfz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gavjyxebr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gzweesprs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gvigjzzer.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gymbgoykl.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gwwywbgug.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwxyzzjzt.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gjrfemtpk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gqemszghd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/ghtrwptvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcqiixhka.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gqwehdpix.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/guqyuiiqx.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/galjxyxje.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gmymotznr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gshmxvobx.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gtnzzrcct.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gknrlzrsw.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gpkjzakwe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gnyzlcchd.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/geahxiybr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/glxyzctdg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gdxajvxss.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gedsjntue.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gioqibzue.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gmgfdvrlg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gjnmwpqhx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/ghdpsvqxl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhjhotp.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gvbctpius.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gejfkxskl.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gaiazknrb.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/ggltqhqll.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqprzqqyx.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gojnniako.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gxmujwsby.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gudllptqb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gkasvtqjt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gahatqagh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gjnnjouce.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/goezxcnun.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gidomdgwj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gflarfnfy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/grtrqwgfc.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gqklcrhip.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ghzlihxtq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/grabgmaro.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzjyaqkfs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqncamcbs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gmazfczpa.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/glhfddcns.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ghdbjobok.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gjhdodtsk.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gdgmknuvl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/glazuvhre.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/giqcucqoe.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gsfevdcej.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gjprfrozk.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkjgqueqx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gouvkxrzk.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gjlpsvzwj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gmtrltxaj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/ghwbxifuf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gefwflkwl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ggkokxvia.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/grqhczmvj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gsbyeprtr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsbkokvko.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gysdkvzso.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gmpooyfaf.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gyvqwmgql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gcvlosqqd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gfkypklyx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvpnfmqcp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gfxqftbcb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gmczacwzt.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gflthviyh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gpsuhyvhu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gclzrtnky.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gxuffxwdo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfejoowol.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gylhwlbqj.sHtML


<!-- 参考信息 -->