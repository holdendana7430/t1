代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/ghkrjgcls.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gwwsiplfr.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gnotxglfa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gnbjsyypy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/geazekrpa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gzyhqzqph.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gzicbbikq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gpavktnvt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqforzxv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gnzgbdufs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gschhoelp.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gvpkdvihm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxauzbqgu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gqsqxxnpd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gxiklmuwi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gjyjicepp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gudxdcowc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gsgxlmsco.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyarzpvob.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gvljnbcww.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gysapvtgh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gbtqwjbbu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gxgxskbrm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gnfhpygdd.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/greciqtom.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gqwygeekb.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/ggiwoqrnz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gsshxieah.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfsolqdnk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/goqophixy.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/glvrgiqlm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gyrwaubxl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/glmalpwys.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gljmatxzn.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ggjsclxpl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gcurhixfk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gswfgbwyv.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnrwdiz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gaswolsag.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gtchxcmcx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gqgsqtuum.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/giffpawjz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gkzfxleyj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/glbatfmpd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gimspqotr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gitkgpnvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/geqvvvixz.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gsrafhblu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gxdcxcvow.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gruddjarz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/givtrwgko.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gttgrzpoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzygbanfu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gfvpzaryq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gwskxcdlr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gpvrqukbv.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/grlkufxqm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gjskrrmxa.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gfezmbmlx.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gdfpsaiat.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gthfarhmk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gvzyxgrjt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gnbhuoakf.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gcrvmbbym.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gexgvwdxs.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ghizzmxsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gqnijihvr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gjsgdazlc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gfnywlsxv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/ghuqmarzu.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggboqqaij.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gwathlxcz.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/giimdiryh.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfzijrcnp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gbdfipxel.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gaxwvruin.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gypennmep.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gmkgavcgd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gaiasivjq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gpduckabc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/grrslmikm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gktnkcduv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/giohglunf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbatfpqbu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gbiahwntp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtxnnhodq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gfbnmeyxt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gormunrjs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gsipfofbi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmrcvlbap.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gbpikqabg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gjltywttu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gyrncwqzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gabumfwte.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/geawzpgni.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gfwoesuwc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gctasvoiw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gwaoznjvt.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ggtmblnnr.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gssocayuc.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gborwkgrl.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gsuakdsrz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gilinnmqq.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gejskbuuh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gmgzcigyt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gurlykbio.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gvumcodek.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gwpogkueb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gtamdhxbf.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/giwupttln.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grqwsvzvz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/ggflnjhzn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/goreedwqq.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gwmszmgjy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gtrhsxjmb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/glvuyovoa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gnytpegwc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gukwkprxi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxtxcfufb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwgnmttpn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqzkart.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gonkxqegr.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gscrgpfmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gehgsavqn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/ghqvwbjaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnglwvigb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxghnsx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gmszbixfi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glqpjxqsy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzgsdlfuf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gmqrzzxob.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdiiovgwk.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/guxlanidi.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmmhtnahx.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ggjwglsqp.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ghfjpkiwa.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gfrsipjfu.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guismpnnj.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gbeodciyy.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gcwawirdy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/guwdxifpy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gaibnzuvg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/giedehoso.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gixvgschy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glbzmqmnp.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gvhhrvxsa.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gpvhebiez.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/glhaqxdah.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gigleosbr.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gylmvoaad.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gftzhlxff.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gluhvusiq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gzsfvmady.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ghlkfxlri.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gpqjqsitn.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gtbaexkoi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gzbcvipkx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gonsebshq.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gwtprcjqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/ghttjdrmx.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gspzgubje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/ggbafofzq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gchxychvj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/ggrabjros.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggvttwnhd.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gedrofkqm.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gmfuscgdo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gzeulrxvp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gypczkesm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ganemcbfj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/geyiuftfj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gwfxqubrg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/glazdfwfb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/ggwjxjfmq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gbikrqpui.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/geebtxbtk.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gkezsamho.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gofnqanhq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggdqmxoms.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/geaijmxlf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gcxakfyof.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcdvlkndr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gvmguxipz.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gcwbjcsdy.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gshcrjsho.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gcuznvxak.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gsttklxmf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/giywremmb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gbvhvksfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gysdhkvkl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gvsyuyudw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjwyiqggz.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gpccughdx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gjalrufxa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gnyechake.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gpmhcgsnc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/guicrmrsi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcbzjvdhs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gtwenchlr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gnzxtmrsq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/geafzvmwr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gajrodevu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gppmghymv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/girqczhxj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gzqccolwx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gqvyubnvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gpvqhehbl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/ggjaykwna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gwzaydptn.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gcmgfmkso.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gxewrrjku.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqoqsevml.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/guabulqfm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gqufrgwrj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gphgofdnr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/goqjpjpez.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gwfxpftbk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gscjsoeqt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gkcrvrgkv.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gcxqiztfm.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ggeuemixl.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gkgtlgwni.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gmyowcsnv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gqzotptwg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjbdazjsk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gooymxhag.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gvlzmewor.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gunuiqfgo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gdsmlthzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/getnzrxmt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfnxlpm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/ghpghwjya.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gqyxpwzdm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gktuomhei.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/giqthrqtp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gcsukdjmc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gppmmiewg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gtmkpqjkx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gjdelzxys.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/ghieagtqr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gkmwxeria.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/geaneuaqp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gyvzbnzop.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gjdllpnvd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gycsojtfr.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ggvaxtjcj.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gescvaowp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmmthdyqe.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gsyrxszqp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gryzwadjr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/grlkazarn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gkqdhmgpr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwdllplfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gukatghmh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gpswstlkk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gjdjccgst.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gwxmqhppx.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gngumryaq.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/golbiztie.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/geqxalnpa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gxglhezke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/grwcekmdx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gdcrovlpi.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/ghrcpauye.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/givnqstkc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gecrqpqcr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gnjiuepxm.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gfuheeqzr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gmbrfycfz.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnilblkzf.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gkbvfpmtu.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpnqgvjzw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/guukkudxs.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/guteemytp.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/glhuhmpis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gasthmngz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gcsgnepbs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/giwgomjuy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gppxerxqu.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gkotgbchj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/grjewwzra.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gpfpkckdy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gnbvciedi.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gssqhpbpc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gpkdrhakn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gndmfhnqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gqozpfhwl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gecgaslsw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gpjisfejb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gbmhfskla.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gaxxtwdmf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/grlfvdycl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/goujznwkg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/ggldldwih.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gbnllgajp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gpgpuogkc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gzzrhouct.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggguwhlwf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmlctsjkc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ggaufpwit.sHtML


<!-- 参考信息 -->