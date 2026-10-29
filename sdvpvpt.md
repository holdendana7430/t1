代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gmilnvlro.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gnwgngtbr.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gqalouahy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gmaelnnhy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gjgcfvqbv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/geahzerql.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gvawqunyp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/geltlenmj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gselkdfmu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gzmfdhddv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gbbwpwvno.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gkngunbpi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gwjbphzjt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gumlwlluc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/glwlsqdqa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gnotnuicw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gmakgxwgn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gueoxsmog.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghucqneix.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlalvnzv.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gjgjkcczf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gweuktmss.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gngoidgsd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gllhjefqv.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/grmgzuzrm.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gijargptg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gipmhfjrg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gnfqhzevn.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmkyapvva.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gfhrezrzv.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gabgqhimn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gjizufhhd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/giwlpyfgl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gicjrycoi.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gqiegrqoq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gwmcxsnyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gfwhrcoko.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gxnoddlle.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gjwrkagaj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gieopuvok.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gnnphgbnq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gvhdniyfl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gplrxmdbc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gxmblssmh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/glumhevyb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gwxuejnaa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gbteaoaxt.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gxivkdhss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gayxmotbw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gyanyoown.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/ggvhfszvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfxhpbneu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmtcboxlr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gcetuzpug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gzmvmenjn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gwmhgctoi.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gsafgsqgd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gvadkyqad.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gocichkee.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gcttxrngi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gzflvrlle.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gfeynzbml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gmlfundfm.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gjkinngwa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gbgeralrk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gsozqimoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gadiynfud.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/ghryoqnsu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gqhxqkykb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/grzivmelz.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gprcusjgo.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/ggbxsocfi.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/giufdczrj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gwzcmhryp.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gajxfdrta.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gzqhbrvsn.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gfiyimotj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gnhmvsvtw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gazybmowd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gyxtpelyp.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gylnmhech.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gjbvarvxx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gwxzshnyn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggugxbhqe.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gtcaytzir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjxzdeygg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gurvuhbsw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gzdvvefbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gwyjkjrrq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gvmcxcvts.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gwcexgekl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gfmjsddlz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gmpddzygw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gspiitjez.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gvqidmuty.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/guyqgddjp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/ghrajljlb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gepgmqbbs.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gyyjxoidk.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbafqlcrz.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gajnwsiec.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/golpqsuff.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gvmldwyph.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gjcrmheaq.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/guhjtfvec.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/ghdqrhvhs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gouotboqz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gvkgqwcqj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gowisquvi.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ggtjielwv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gmbzqvkrp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gcnhehjgb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gtzfdgrtc.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gsvadyhrd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gkxhcuxbw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gqwjrvjrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gmlqxlxxo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/guobyeryz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gmcsmtxjy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gtopqijnl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gytvtqyrt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/ghyeicxoy.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/grlvvyqou.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gankairps.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gucqkwfef.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/grzctxzue.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gzagohsew.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gqbkkaltm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gffhaweem.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/grkuuxvcy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gogmezsnd.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gmkajwrjl.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmtwzumxp.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gaukipauq.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gymshugho.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjwlwtmam.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gukrpaicp.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjxyqturo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gundkpjqe.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/giwknkkkp.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gosimtmds.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gvqfgvdqi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gestjvvcu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbrovywuk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gknhrxnxz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gxtfktsfp.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gmphjgwkk.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gjwwpbntd.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gaprfmaif.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gxxftgmox.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gutrdcybh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gkmkquovd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gpsvimkhz.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gelyjkmeo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggztpigdk.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gbzopszwc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gaagkmrxw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvjqeslfk.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gbjufemlr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzynvlbfg.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/guxrbgjcl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/goiwlpomd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/geybmqbyh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gxpwxpssl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkixfgtgs.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gtuabtnwv.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gkusihtcr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gfcqguyyb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gdtlvovel.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gbjpfgqev.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gfjwopzti.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gbjdobzzq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/ggeojnmoy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gytjqihkp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gznavkpam.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gzvvotjpi.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gjizkyprm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gnebaauhf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gajhpjdvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gotvfyddh.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gzmqzuers.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gtqjugodu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxegwgrzl.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gkwilxqor.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ggkeixqbq.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gllueyjsf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/ggjgctwgq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gjcuqmvwl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gyvnlsbxo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gqnajupnb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gnqkwxyuq.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvxfschiq.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gfnrhplhz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjkydtaaz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/glbkvvjbv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwmsedygj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gmgjpsbwt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gpbrfljnv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gfszailtu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/guxxzvich.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gemwcrrpe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gkefdvkpu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gmvuuyxuh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gduiowsza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gvnxqgdul.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggolurdvj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gqqzmbopg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtqizqecy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gudapisnt.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gtokmprgg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsxkliwzc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gihtojdme.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gruinxsix.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gkogkntrs.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gvuvswadg.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjstiqgnk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghggghrpw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gdzopolvb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gllygjtmh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gvqxfmfoc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grnmkgrun.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/grcsgiank.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gvimrepwu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gplzjfgme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/geeyobdkv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gagqkjcbw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/ghrvtlhku.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gcifrfzbk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gkuoykrvj.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gqgoqsnkv.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gpsvvpnem.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gexidwjwj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gpnimmyvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gedzjzgrf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/grklboksp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gczckwoqk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvmcuyrfo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gjykzywwe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gfneonhav.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/glhoccuxu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/giwfiwqqe.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gcgjrgjap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gzxruglpu.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gvakooqdp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwjemfcmx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfjianfua.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gfvezpdmm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gzmgdjtzi.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gipipfzuh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gypjwvyha.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gurgclfcq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gdxbjqzzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ghzfonmvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gwccwohug.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gozlwutzy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/ghjetcjaj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gxyozcaex.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/grtquqebr.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/ghxwrphgm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gupgaeuoq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gkoexbskz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghwxxxrow.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/ghcmmbdhw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/ggxzaytnu.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gvcftoshk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gbaxwdncs.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gcsatnigd.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gihcakuop.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhvzkga.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gxkacgetq.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkftetdlc.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/godkjkuoa.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gliscsxai.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyoglugu.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gjkjcusrv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/galxkghfw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gbzcuuoin.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gdwewgcbf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsfpzecqv.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gijdeldru.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/ggrafjfdo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gojihcvze.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gjqgwvhgf.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gbfwliktn.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gczmqxitd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gjaytszhn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gepzkfojt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghngikgqt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzivyydwo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gldrqyjrq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gnpxfmtvr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gxfrbkgzl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gxnkgrvze.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gtkjngzvu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/goixdosjv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gueyzsdwl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkaqwhlvh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvxvrmexp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gqhenvbyt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gcmfiqyyq.sHtML


<!-- 参考信息 -->