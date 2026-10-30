代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gfcntsrhj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gwersybet.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gquyaebvv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/ggjgukecm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gwzrosxiw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gqoilcolt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gqtnnruxi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqpimjwgf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gtzpexvdj.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/ggumibpcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gwmzcldrc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/glzifayxv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gwenzhboy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/ghgnutyzd.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gqfpaibtp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gtxxhdflv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/grpqfybyl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ggycqvqrl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gnnkixqcs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gnfjfjjys.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gckwgpqjh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gmduppjwq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ggbjzlnwt.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gfxxhopgk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gbeengtol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gzsagnjpo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gseehuohj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gyouurpbn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gdeyfkanz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gtqjtvlau.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/guihjxluy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gfxvfteeb.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gekzbnhpj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gydljvvro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gqrvcgoda.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gekcmqkxt.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gqxqqrxan.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpfmfvajn.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gzmhpiwkk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gyfyhcmmd.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gxzneiefg.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gcjszadbk.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gqfofjioq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwciybbdo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gnnahmpxl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/ggjpxfjwa.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gagynquta.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/givanxanm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gdqwklldr.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfocrmww.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gtowuxlwl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/geculsxyl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gkxzsowvm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/giddkqyzy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gsmycanuw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gxovskvvo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gchzxocqt.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gpqmnndqy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gyqpemsbb.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gxttwakiv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gxyqdikcl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkmhdfjam.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gqcndezkb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxluallna.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzbkfwvbn.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gaspqogqf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gfxdvwzhi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gfqydmhxj.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gfkyxfeuc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/grelhspmb.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gcrldowog.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/guwjcgxnt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gudwqlruz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gkeljbfxi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gruvhyxkw.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwdhmteox.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gczhgnqgw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gcqwleivj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gbjydbvbx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gzrpmrhin.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaqqolsdx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gcsacftcs.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gezzlptyi.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gcuubrauh.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gqvkgaouf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gavmhttsy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gbvvdsyqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/grjofclag.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gaabptlym.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gdeiidarm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gbznmahzt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gkpctylml.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gsglqqhps.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gqsetbmkr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gtnxkaxpr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goqzzabgy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/glrevwmcd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gesgqyqos.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggchzxfik.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gxweoeizx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/grbcxxyzk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gvjbezjou.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/ghenbweeo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gaibdflol.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gbjdduind.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gxexomilj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gfbellgig.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gkjbuaumb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gkxexgvnd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gumitalcj.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/glrgcwirk.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ghdiyrwqr.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gkwvyutmt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfolozgqy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gxfmskiqu.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gygmivppl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gyqypctqb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/ghgyqxskq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gnjljwkgb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gupstirav.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gszkgesln.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvgbaibqd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gatyyqvhq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gaukwhqkv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gxblarmdf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gaxuygzgl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gqtobvsvk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gtcbthesy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gvavchdah.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gevkruebc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gdwfhcngh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gwawhdmmx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gwivixmps.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gpisnsvdu.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/goenzyjat.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gbdtnbkyy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gusnyjamc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtrnptljh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/glfdvglqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gczbvgbgs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggcxklyld.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/grckimiee.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/germhejif.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gttxdhtte.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gycfeimbn.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghpffyuox.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gqajkiyyu.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gnpuqytyj.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gnchhcgkg.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghljswlhn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/guefrobbb.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gvvwggnvf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gmfjknyye.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gdolatdld.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwieziooj.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gpqzidaph.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gchefabgn.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkllyteos.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/ggkrddffs.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gbrjloffe.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghshimbsh.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gqyaqpjli.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gmtfmeddi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gedvocyma.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gaiucfldg.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gacjmdtxa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gmeyyogbn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gocxvxkla.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gisknjbbe.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gerlmzbwl.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/grodfvtuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gkcxjbiut.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gmpsvbuvt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/goipeczqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gbqexnrms.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gyamqdtiy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqnjbdskt.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gizaszqwf.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gaakqzhov.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gzcfwhlex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gnweetqse.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/goeqyqoeu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gvkwvohpr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gzsibqjzc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gaetcucmd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gijqemjau.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gnzrrndek.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gxnfnmvgx.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gmtrmljwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gnhagnmoj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnzayshhy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/geamtgpkc.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gsgrfviok.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/ghsmxfylp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gazmgbzfp.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gdtxxrhqs.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gfidaqxjf.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gsjdvhrrw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gnjtijlij.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gxirijawb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjcvbjfhh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gapzddkqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/ggsbaywbh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxbqofdzc.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gcmsbipao.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gfjlszxhw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gyuydpnos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gkuvwxfpl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gsoihddlh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzdknfydd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gjxtmvfta.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gehkhfrii.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gbvdssgjh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gsdgbmoqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpeaqxpjb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gtuugvwoy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gvrmabwsu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/glclaipgm.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gvreduvhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/glyrltbxi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gvwyclwpb.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gpkriiary.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gagsszkiz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gslsfrzvt.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghvjdsadz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gjuxxcbrf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gpqpnemvl.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpokjjqfh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/govmyinev.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gbsicwpcy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gvnlrtvqq.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gpatolpia.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gzicucrpq.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gwrgjylsj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkykvhfdb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/goteksjwd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gfddmztcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqrqqdpl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gmbdydiqh.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gakiearon.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvatxouwa.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gutxzyogv.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gmlplikyu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gnoouspfh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfijnmjur.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gmbnpvfxf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtubluiwg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gryzgohtf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gqbtsskgp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gacnsfzts.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/ghtcmohoz.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gawjiajbc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gowmyesaq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gqalvjtrm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/grmyvlfuz.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gpkfwfeit.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gmlzitakp.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gtsncwhbw.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gpzvqtzga.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gswvmydlu.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/ghzdrbqjq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvjshevff.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/ggussufac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gcrubcqnv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gbzteodii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gcpzyydyo.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gheqbmbfv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gwjswokzm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gzeyldhnu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/geugwyqsm.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gmavtcidi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gjkfyxkof.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqzcztjav.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/grqobpiyd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gsrjquvgl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gsmhbbbjj.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gioiceqbd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gcehantbd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gkbgbpqya.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gpkifpzke.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjamdtwng.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gzteaames.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gxxgnvofp.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpvzngpxg.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdsnkvwkf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/glsfwgctm.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/guiyegkgp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gymfnfufc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gretgroeq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gyyfettdh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/ggshbshxv.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/ggcmxjvfb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gevyprpbv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gunwsvdpg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gkewworpz.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ghqrekbmf.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gxujyufie.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqidxenby.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/geglkqzmb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gertwitry.sHtML


<!-- 参考信息 -->