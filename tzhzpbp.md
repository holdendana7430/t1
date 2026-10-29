代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gnnljzfod.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gczdlujtu.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gswhagczo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gpdyidybg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/ginqjczax.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gkgmsrcxu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdvuxlxas.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/giuznywpb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/guqivkunz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gdsbhcdar.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfklnwopu.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gjvenutrl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gqnhladpw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gxyjitaoq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gjpusaukj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gtqzsxjyy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gxucsjrjk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/geqymnhaj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkquixhga.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gkhawujmi.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggnommpvs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/goucsyyrk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gxfuzavvj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/guteaaixk.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gqbvczlrz.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gckysasvm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqdrxzk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/ggxluywqj.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gtadzpqkm.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gjwbsrmrq.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/ghfaweeze.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gyqyywqhd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gjulzhpql.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gzcewwzpq.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gmpjpekdt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gvqqdnsio.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gkvhqvrfn.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gdboqrsuv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gbvqghmrj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gszfntroq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/guulutfqa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gjwshunra.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gsuljjksk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/groduspvb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gpuhrjulb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gvzfmvdrf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ggkqssjqa.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/geamncfjv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gltqqaqzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gymkdvvrs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gfecssade.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gdizklqzr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grzdykkco.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/granbwpeu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gsjchvsgf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gyfihxeyj.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gxrfttytk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gmnbuvhgh.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gtegbmkby.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfeacdxvd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gojcyaaka.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/giwhnkbak.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gojtovozr.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gvoqxvnub.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gwkzjhghf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gfppotkkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/ggpxwevxy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gpuwlcfri.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gfnrynemw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gnaezcxyd.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gvdxqznlm.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/grlqpnnap.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gskavcazj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvnlhqxl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gzoxxreis.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gvuvtellq.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gikwhtlnw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/ghnpilvyc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gwaejcken.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gbjletdsf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/girsdqxbf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gvozbrxgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gnmdqelji.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glutuucsz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gshbfmgvm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gylsopeia.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/ggnpotrqa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gbewefnzs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gfpjwnfcb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gyvxolgrt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gpjocsqly.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gwvuvvjbm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gfzjabrol.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gseposnsx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/grwhgmdtb.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gvdtjkszt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gwyvqbyaw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gkvadnfnx.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gissezfri.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gchpogwtl.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gkrpdvclr.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvhtixygs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gqdtwyvsg.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/giwniyfft.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gxywxqbge.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gnepxwytv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/goepfcalt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gvetvhvmp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gfnqeytyt.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnrxncuhm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gfndrjmvs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gribvwhjn.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqhrofpas.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gmgihvmpk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gjjpemsys.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggbbxxmqz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gpfbxfzbh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gkndfsnvs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/geabwwzmn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gagvqnzvi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gceqpyubp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gkkcixhfu.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gaocqnxhc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggrthykso.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzkwinwtp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/guwmjeppn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gbffnttmg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gxzcwxxuo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gixgkkzmm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxyzcazai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnbfoihth.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gogehiucm.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gihndqdni.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gnorfjzld.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gyyyfvzbq.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gzquspfbv.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gwjvvpbyq.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwfjectsc.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gjqrgjqni.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gzsmpkphb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gnoccmfbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gghqutrbb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gebfixeqf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gurnhlokn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmeiqlvzm.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gbbxsbfuq.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gqlkqfqyg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gggzjpqcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzgnhrpkt.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gdohvickd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gjpzsupaz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gzhwgpmiy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/giqsiblvq.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ggttbsdmy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gvsaefwsg.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gkjavtrov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gcnhdnkpc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvitscocs.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gzxbwtepg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gnaybxvrj.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gphukwsga.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gzcxihyyt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gnvuzqamw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/groybpjwg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gcozyqyju.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gsphkryxo.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gefomqkpk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjxfwcs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gjchmlztz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gwdygchfj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gfgfheskl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gwloixebz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gpfzymzxd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/grmshuuky.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/guxrmsjoz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gtttwasmq.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gcllbiuyc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gsnyjjoap.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/ggszxqpep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdeiqyw.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gafhrzyjq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gywpxbgwu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gwdehiwsf.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gvvoevzld.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gjpsqdxyg.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwlngkkeo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/glkcnivkx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyioolihh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gnhayylix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gopumipkd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gpvjuogfn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpwkrbfgh.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gguvjrhuf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gbkqjrhxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/getjkfrcn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gfozefrzg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gqpszfvxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/grltztvjk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/grgygnouu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggzbbfaxh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gvfnhwrnv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gloyzwemj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gvqjfpljd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gnrndbjnr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gatircmwr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gungqllgf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/guvuxpvgi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrnwyjuq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gwnkpbhml.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxxubehxk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjlvjwkks.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkybirdkh.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gbhbwlagu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbvoexzdl.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gwdyprdpq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gybfslvdb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmkletlbe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gnifwytpt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gpjoqumtl.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gqltpgwlk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gljflgvns.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gsdrrnqrh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/ghrnctfzb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsinreiuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/grlcvznyq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gzkhrusll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/ggjfgvbvs.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gxuhfstvi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gohawsosp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gwiwgykpv.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gfbvmkhhm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbmkrrtnv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gseeysdga.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gacngfpvu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gndotdooz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gzdwkchwy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gzaepdotq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gmtqrppmi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gkyxducpr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghqyaekfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gvwejmpmv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ggghqquxm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gougnxlqy.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gnuxycqbi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsepxhdym.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gdiruxxba.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gxlcdvith.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gapdxqpsf.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gvpxzcwyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gugnaprlu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gkhrrlftf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gslyeaeko.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gzjprpaqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gtfbetnpm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gsomjwaby.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/grrtdeuuk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/guyspphwx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gtmiiusfg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcrcjgna.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/glexxvigg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gjxontnae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gydgajvym.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/grlujbbsn.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gbhjhwwsb.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gvminqnkl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwswhuqea.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gxrwklbll.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gfdxahygu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gveossbsn.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gkxotyvyo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gnytqygxv.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbshyegzq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggzpgfvmg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/goxwtzbih.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gmndqxjhj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gnmgwaaql.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/goyvzknjx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gqyjwqvih.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gsrxogmbb.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/goregyfqa.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gwaglbnij.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gnowrdsdt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gaqvanjhd.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gduasaqww.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gzdizmavk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gwmcugibn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gaoijwxpl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gracrrqus.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guoiphpvt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gqxequecs.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gysmkcuts.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/glfsgngav.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gxodtyhfh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gsxikydyy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gbdzevinu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gzxionbcx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gkoigehgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gknfabksg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gusquqopn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gjzqvbeee.sHtML


<!-- 参考信息 -->