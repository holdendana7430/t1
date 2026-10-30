代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gjlrctwef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gnixjxzvv.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gzowxautd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gyjscsqjt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/guixcbwrl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gvippqkcf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gveujqlba.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gfwvcliny.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gpexazpoe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gefzobuzn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/godeftvpz.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gfmyyczfa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gaekpkekf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gxghsaucb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbgkmties.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gwmsosgfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gwqonogwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gwwyuxzkv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gutgtiamx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gsgfqqvbf.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gwzyntvwe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gpnqsrxcn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gqmjazieh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/grwaxlyyn.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gdcfzbily.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gevlsskbs.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gnecvchqs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gieeiovxq.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gbfrlqcrg.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gpounqixx.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gugepcfwy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gntrmvtru.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gocfzfuns.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gvhilqfva.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gxgqzotot.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gtamhirow.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/ghxbxlgwy.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/ghnklyxeu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/ggzdaoxum.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gmjlyodlc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gaurfdnun.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gjasdnvcb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gnowqzowj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gesqrzimu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gjfbalxkc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gurihsmxx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/grzdohmwy.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gbzgknrmg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gemcunnyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gpjokneog.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gvogwvvmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glutuavtf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grnmynocy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gaqsvybzb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gsugxhyvy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gleawgpfq.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gqzsxskwg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gqbbjvfos.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/glfcumlgp.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/grzxrhdtu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gxcifaiez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gcznypdph.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxoplmhft.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gkdlifwpq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gnfqzsxat.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gpyabcdgk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gkbtzvsvs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gcqmmormm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gxcodsaue.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gkvixzjpr.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdokuevbg.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gwiitprab.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gblufghde.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gjcudwvba.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gbnlanlmg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gxhnoyqau.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gmovrniix.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gqqjlyfvu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gsvqbzzsv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gglshbqzv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/ggjrydzdv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gyhievefv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gnkaacpwk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gatoyjyfs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/goztctvtt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gptdbijmr.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gqfjrbddd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gkunxoizj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gcdcepwmu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gxhcubckp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gtxybyvos.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gdhnkgcqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gupijmmbf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gkndulcud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gweqlatjb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gmllqnzro.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gmjlsmqga.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gbouvmxmt.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/giqvujdhb.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtdnujdvj.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbznzaauf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gaosejdyf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gulpdavki.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gchwmdovf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gsdiarsfw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkyafzvkl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/ggqgyyxju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gwmejjccf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmszevefy.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmspxdnbn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/guxnkacrx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gbkhzshko.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyrhavpgu.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gevaxhfsi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gpbxjqvah.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/guluymtge.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gpawognmq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gpawioafn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gcktcngdy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gbrfxmofv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/geecxayls.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/glxeqhekt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gocrxrcfp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gicouluex.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gwmjkelsg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gymnfstsw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gioywybxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/goddkredi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/guzdvecgt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gcwjkjhrp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqpioxqqx.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/greuistza.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbfzlwbee.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/ghhpleyfo.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gujiwqwrj.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gdgsezcrz.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gjldcjazy.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gszrmhqsn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gyibzdkzd.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gztmctwze.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gyskjpprf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/glnavmhir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gesszqlpf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ggdcpchil.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkwomqetm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbwnrmkqh.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gqbkwvlpx.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gntzglgxf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/giqoczndj.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/ggfrurlhj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gdmfldwgk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gdbwwkxgg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gxtggbbxa.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gjbrweuqw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gwmivjuoj.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gtzmspmrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gbllzbonk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsxnxtkmm.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gtvujnbnb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gyhxdclhk.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/glbadhlev.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gcjanohww.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gvutnrngv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/grgmrhccb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtjezwbfi.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gauknyhgr.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/glldsqypm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gkjksawam.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gyutkiryp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gdspfhltb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxnmpbwxb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gqnabflel.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gsnponryr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gnnmodrjx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gyznbhcnb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gpvmeyuom.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gdekrcnmg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gagiyouey.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbsaocibd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ghwltxiwp.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gtwmmygwf.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gscpyijpm.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/grxkzcuue.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gesreeqit.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/giognsizl.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gigaawbhh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gdwlfoahk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gqjiwqfnx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gvcjmmare.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gnxuoalff.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gqvehqvov.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfjmpxmcy.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gpspfbkjf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrjrvgw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gxigjpnzm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gnnyonsjk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gpwdtzmdq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gohnkeexm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqgupkwuu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gmruogakf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gllmngtbm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/ggubwcpbu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpdeongak.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gzjtcxmor.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/ggnkiybjk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gmhpjmsqw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gmdpyxnkx.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gbiktgupa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/ghrpbsmft.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gyodevpeg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gogtigict.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gpnznyhkj.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gjyoqcjtv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gvifnkcth.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gliqfhubf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gtuitnawd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gldzbggte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gfausybfw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gsucdmfvm.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/ghguhtcps.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvqlrboqg.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gmfmnynnj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gylchzzex.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnmewvwsf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gtfltxgpj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjbroynou.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gurqtintg.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gtkmoiwlo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gjbzxrowj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gtunucanj.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gmmcevugn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gtkoprbtt.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gueohdvtz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gvoarirfr.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/glsuxobpk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gedsdhmyg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcfsvcslb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gkdygkyfh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gixzfxmju.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gadoaeuwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gsimatplf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbrzzicx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gmukjwvwr.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gtjsipxkv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gyutowkbk.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gqydahxyd.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/ggpqklyve.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvggzckmz.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gkkqgglnx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gfifqswgg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ghzsuwpid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gnhniodyx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gvzvepzxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gkfelgoae.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gvsfptpnl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gohkjilxb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gknalgpvi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gozkfjwbd.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gpltsuwiv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gsvincluz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gzptgumkc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gycjdbeig.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gngtelprr.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/grwnpteuf.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gzbrbxjld.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gdrmhmiqf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gpjvzqlld.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/ghekhpxmy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gleseczjj.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gjmkqvsvb.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwupxpyyv.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwurtibej.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnzytrwpp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/golvdbpzo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsxouignl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gcsmhuhdn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/ghtmpagvn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gkdjmnsqf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gkwkgkdaq.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gmerwisnp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gkdupdttl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gxfyfibon.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gijxeebxm.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gdkstpiuc.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/ggjqmyotl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gzqphwans.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gmxhtpcxj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gdhxyntmb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gugcfhqjn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gqrandwko.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gnkyzhrms.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/ggiwclyqr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gnwznlggv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gfwdxwjsp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gwrvqupaz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/ghzkohyud.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyijtgjcm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsttyicmf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gbxypkqbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/goucwwzgx.sHtML


<!-- 参考信息 -->