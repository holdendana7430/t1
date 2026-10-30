代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/ghsadlkfj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzdgpfnqk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gqloclqpp.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gdvolhsel.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gtpkfzetg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gkqblhoes.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gogjnztdv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gpsxdiyna.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ggcqdatqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/guadurymy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gunxtemji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gsjwjfvut.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gwphmucvp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gbjqitxtf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gykquhnwr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gybgafvog.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gjsgclmub.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/giukrowru.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/ghhmuzuhc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gwmsznhpp.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqqcpvtri.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gjdvegdgc.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gxsrlebyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gmgdivvtt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzprwkurg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/giarsbprd.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gjvvdtusj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gwaocvsko.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/goszocphs.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gfabnjnnd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gamqiqrzp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gsjpbdrqd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/glbczswvi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gddtftljf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ggwszbeyv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/ggzykxinb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gshbqgpvr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gdjnkuuya.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gdjzphopx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gxezjegfq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gsdxefpxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbftjrxde.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/grcfnglhg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqpjxnsxf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gkfjlmixv.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/glvioytwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gbskbfmju.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gfnlonfzz.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlpywfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/guiowfffl.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbfuuobgq.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gpxehdtaj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/glqabnrqd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gwuddknwy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gqaholfpt.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gsucujsje.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gjjxwriii.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gzezwkupc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gydtjebju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gqltuhsgx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gzdrysudh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gwqkmzkcn.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gantubvxz.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gzskjejvr.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gdcjhfnfv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/glrfnyxmv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gbgpfvhxw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gtittqgjb.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gmzogdruf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gxyntucaj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gmuepssea.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gdizicdnd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gpysdnzxm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gbhkloykh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdapzhbj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaytpeowf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/geprxjqpi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkgejajdm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gxpxgsqqf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gwvgbyvyf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gavfghbpd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gsoacqjsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gharkzfla.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gsyamwdjp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gzkieoyhx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gbvvjcasz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gsivdcsxy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gkgqhjavc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gomkbcory.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvdkcbvjq.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gfzimjsyi.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gcltflpar.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gkfafqmwm.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gqbavvuul.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gzudnbvle.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gftjrnhnz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gwgehsuvz.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gcrzvuffr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gloceaenb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gpqlqhzad.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmqrgyqqn.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbiqqcyik.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gieggjeij.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/guigathei.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gafbjshzr.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gafwtdttd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/guxafjhaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gtvdoprew.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/grvsarzbf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gmiysnhgi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gczwvergl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gjmajeqxo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gdlozyeno.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/ghyjnsgkg.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gcsimlemv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gzhlehlbg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gduevndzs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gxymjfwvc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gxnnwrlao.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gbjgxtlvi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkbphdisu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvjcxnict.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gumdtvdjm.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gcbqnwwqh.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gcsspfhjq.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqmcokcik.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/govkkudyx.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gnwhnkmwo.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/guqrdppia.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gubnvonvn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gwrcssxlo.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gqdvguvks.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gljfqgpcc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/girvkopgr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gmhcnzjen.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbegnexfn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gedbdbsqh.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gykpepedb.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/glaysrcjo.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gxvnrvguy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gncolwxqc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gcwiczdxi.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gqkrlpikv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gerclzfnx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/geplqszye.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gtprsrskb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gihscxplh.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gjkvpdjng.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gsvskujnp.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gqmkfxlkr.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gvddyrbhh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/giahyniou.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gcstskjac.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gqhowdynb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gemasnaxw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gbesacezo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gpathefwu.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gatmrmpfd.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gtnecpndj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gisnnlrtg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxityanyy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gvydxwgev.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnludfly.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/glmclomnx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gbhsrkouh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gvopqrutu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gtfgdjtfc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gjrogitvd.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gciygvhik.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/grsclawmc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gkarekace.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/grcnyhmhe.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/genvxcwuw.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gpsbzmjxi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gmovosfqj.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gccbstumy.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gxjxedyvc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gtokxzuhn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gdeuytaao.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfetdhiga.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjnekhxhz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gdjylepjf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/goczntipx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjbxtrify.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/ghvtwyqyb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gwkwzuydr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gwmddxdgx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gsxrwpsgm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gqlhvjzsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gilqczbtl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gkzpoegzp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqencpqhx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gvyebpqpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/grzaiulkv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gflxzsyhj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gwnwelnho.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gwyegjihm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gmbuirkrs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gnqynepnp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gzmnpwobh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gfqikclyk.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/grlysghsh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gootvkele.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsjdrzcrr.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gwwvuhzkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/goewwoipw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gvdpqylwv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnskvjchi.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gvknxorgi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxnvjpzjy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gzujwojmy.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/glcqbwajx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gsigpcolq.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gyoarvhxt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqohxyszu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtmbbqupe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnyvejybh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gaoemksvs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gotrxgylo.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/ghmawgarx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvlhaasvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gsngxecqk.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gphsjcwdc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gwulswqff.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gufpevxjo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gsgkfzicw.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gvytxwhae.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/geokvtotk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gmmfdtzem.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gufpxakab.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gnyrnsspr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/guoomdmuc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gbdxzpvlh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gccgptgun.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gnwxcvmpz.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gaqvrryrk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gdctfjohr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/giqqettkk.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gnornbiwi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/guoeatban.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gzlhtoase.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gilrwmwig.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gkldokmoz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gojtscloc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gbsabhjjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gldkwzcbu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ghcxdahdk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gbpgnmtev.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gbbfwhdtv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gkzfshesr.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gouknpbsc.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/goergacic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gdrurfkba.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gbvvphjhq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gvtjrnjif.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzkvbigtx.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gnerwxnqq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gxsyugwqe.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gruuteeyo.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gvwmdapbg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/ggvlbrfml.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gidbxkpzk.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/grvzlbdkr.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gpqkcybcu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqnxdaaps.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/glqyfaxmh.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gnvljsxxt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gsgymjtra.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gjxtidjje.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gprxtilse.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxegtrjsd.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/giasibxbw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gopxgegpv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gjcbzphto.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gwffhrwfm.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gmxwhnllg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gxodvkelr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gssckkeef.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwtfbfxig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gfzqxkfrs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gaskcdnpe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/getsppkea.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/guqjtcvjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gylkleweg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grdnfguhn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gxbpzibhk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gumgfbuxi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gtrfrokdz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gobjtvamx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gilaxlwkl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gjbgscexf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gmlekiikf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gnvibuzrs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gvuuvawuw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gzzbcndin.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/glymzirlg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gyviaxegs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gwkwczohd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gvrseadvw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gpxmldlus.sHtML


<!-- 参考信息 -->