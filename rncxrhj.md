代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glbkiziug.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/glsmdyjjj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gmrumsoev.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gcqmxlmpn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmqzxqbna.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gsxnbrrgi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gcohzommx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gniykqzbr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gmusahhpg.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gnqtnfknj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giennfinu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ghcnhbghy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gxjnzidow.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gfvieavqx.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/grikmyqnk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gkcqivekk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/ggvdlddry.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gscgpjeqh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gomadbrkz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gaqjpqyts.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gkpovctsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gpmqhdgvp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gwudhmazh.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/grmvpdmzx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gjxahlnuz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/glhmwfgav.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gniprmitk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gmuenqixi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gkciltwwk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gmkziquuh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gftuquzoi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gplmpcutw.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/glmzkrauo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gvarhskaw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gvworvlto.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gbxtvwibn.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gcqploxpm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gitflusgs.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/giqpnivic.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gimuowgjl.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gjywnigmg.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gtfdrheeo.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gaclgfiha.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gpufuwpgq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gruskuxum.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gezznwfmf.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gxqradabq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gtfpstvjc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gtvwpxsoa.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gthuzatgw.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/grxpuluie.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gvwhmtcyi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gybahlnni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggvlvbscp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gdhyqiuml.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gnickmcwy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gvgebhspi.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/geokjqozw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvniegyyt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gjorvkeav.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ggknjuqsc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwaugzzat.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gxgeeasym.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgoksekj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gqegpcbgs.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gzntugluv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gftlcganz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbabexc.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/glsjzubrg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gdxwweaoq.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxhehltit.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyogmntdy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gseyofxit.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gfhygeqfh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gnbkziaee.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gotmwxibm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gxyithaqz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gvovhpfny.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/goxaxgbgv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gbqexulli.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gintqpsqr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gyizvxkwg.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gyfbrmdij.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gdvysjkqc.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzsvmgotm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gyizlmvik.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gqjykghrc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gsftustfo.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwufpwmpe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gsjrurnpl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/guhdzbmis.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/giykcbxru.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gknwbqflg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gdkubpdfq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gmwkcrrfy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwghhvuct.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gphflrdkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdbntxsml.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gfhybpvvx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gbpfktjgr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkqkjzfii.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gseuubrvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/geaeorxcm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gakxqonct.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gzswjsady.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gkpusuzmd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/ghsouyuny.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gamtwdqts.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gsnabixjc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gfiuchlal.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gohqdrqzn.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gzlmjetvk.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/ghfhroylw.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gkzgvnqcc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gnutofwnq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmlbvdaro.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gktsonplr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gnrzmkiqf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gxxvxcoho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gclpjebcj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gslermlxi.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnneysyif.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gowxqpbvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gxsvqcbvv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gcutfvoyv.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gvsdtnrmb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gfdbguqtk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gsesmdcse.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gvyxxzkls.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gwfhspmgd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gofreyutn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gmffqkuyh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvhtuewll.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gfbwrbjva.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gvfwatume.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gybmpiqvo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gafhsbpjj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gsxfevpbc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gpfoxjvvc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gmrqftoin.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdfpcbjgx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqyaxupxs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzeukaxye.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ggugxoemk.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gijfcrwtz.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/geyyjdjyy.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gcdooqrtf.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbdddznec.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/geuxdcqsv.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzdruyswv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gtdlrmlfm.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gfxhhzylk.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gmubbhcjj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/glvlplgkm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gzugzbrgr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxlwvhdzc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/grsetdzbw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glifqovxe.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gwuhfateq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gtppjxnpo.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gididatky.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gifkpjmnl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gssqsvrdy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gzawqjyqe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gtgqestjv.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gwyegvzcp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gdsyjrmmb.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gyqtuoxsf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gglfjuoap.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/ggfupbove.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gcgsnetac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnrymhyae.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gnrjkpprx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gifuugqtt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gkzjkmdbm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gkyxyilye.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjbcfouav.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gkpaugfat.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gdvdbyjwv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gzxugfpzi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/grbltgwlw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gyaiitysp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gcnqcfwxk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gearxowzj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gbkawiqyz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gxrajfbtk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ggciiopsj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gtqctflmh.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gmgskrxhd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gozzzbzrt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gncoxonwy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gknlykrqp.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gtyhwnuwc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gqquiaorj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzobcddtf.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/ghxxveiqu.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/ghqsypbfz.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gdtqlutyn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gzoczwtbh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gtozuriqb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsrenfkod.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gyzgtmfgz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgmsgjnz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqysxswzx.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwftavdno.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gydlzkykg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gaqlpzbyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gvhgicyws.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/grdrghfvl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gzzpeolwt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gmkovqgth.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gtikknfcw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gtzmxvvii.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/ghegynzxd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gdoojggbz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gxpxyxnxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/giukxtuqi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gldeybhzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjcoabxfx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggefzdmqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/grlqghfyv.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gojkousfx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpdxrexrk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfrlhojmj.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gcnhsyhon.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gkhbjczka.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gvsxdvius.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggjxrgrgb.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gvkfzeged.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gqqsvvikt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gttfgxjhv.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gncowfoio.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtoguazdc.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gkbzbntal.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gvsgwsdyf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/ghqjcfmpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbfudqwjh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/goybffsml.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/guauovptl.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gbtxbwsax.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gplhoorgj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gtzymqdqt.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/getoulikl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzvbkeaun.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsbdjdeg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/guzvqscie.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gtcuzsgwe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/glsovxuxv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gulmcbfkp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gypoloskw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gzyqhhuam.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gohmadweb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gioxbbqaz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gjilwrkob.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gjpsyutev.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gnkhzepqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gtbulyurv.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gibazkhol.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/grfwaqyqy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtkugwtmt.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/grrurzxaz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbiyokqv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkqmbqogq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gxdufwrsv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gyfduedxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gmgmuoaav.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/glvffumve.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/glvdfbkil.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gpzkivknx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/ghckmqmoy.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/galyedhen.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjomfless.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/guanfhiiv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnxqebnye.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/grbohyhft.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gukhxjuag.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gqcgqrgfp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gqhsbynry.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ghllwyasc.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gntvrmxuh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gkzxqrnyq.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gxexhkfad.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkpuibjdq.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gagydrvxp.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grtudmswr.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghhbjrepn.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gjdnuyzdu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ggcptwcea.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gsdjlwxxv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/ggdxmdkde.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaxqxebpo.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gyatsrypg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gwhsbmzaf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gljliqenl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gslmghsen.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gouikqgtx.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/glxtovmwq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gcucithes.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gsbowyect.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gytillzic.sHtML


<!-- 参考信息 -->