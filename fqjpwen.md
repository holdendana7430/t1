代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gzgsnfqtd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gbmyjrxif.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gcvtotwkb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gmvjlugwl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/ghddgagtp.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/givssswnm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gggyzpwtf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gwucsercc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ghfjaoxwf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gzxwcfqlx.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gmfdrzoxs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gmhpcsmnz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gxhifphct.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggbtznvjp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gxpreeagn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gqzimncfa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gemednqnm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gqjsmonng.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/ggpwigqdw.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/giuduyvzg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ggssqmnjg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gzxfcuvrl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gywqlvlic.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gdogstgrn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/grzbqfpfe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gwzatxbjt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gqtsfzjio.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/geysvpmve.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gzaxpeate.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gulvkqiky.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/geyahxlmj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gcxapnjht.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gmppzxhnq.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghqukjkcm.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gucnzelyo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/giaqxzsgh.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gvjwfjjkt.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/ghkxudcaw.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gphdqeets.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gleevvdpo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ggawjarbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gsxdfbwiu.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/glpnozdjy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gzyrqkocg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gpbmuzfun.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gzjdqzfju.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gproaakjd.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gjwqfympd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gdldeumwl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gebxbduou.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gsiupwdeq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gdnzhftbl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gpbyibaca.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/grcoetdyn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gfaqjcted.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/givuqldsm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gdsgzmixy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gevjfihoz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gertpuasf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdkzremun.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmvobljju.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gyutfwuyd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gmokjmtbo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gnfryfuje.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxmpjartf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gzgdozybl.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghlovsrhr.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmqudxkiq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gsfvpbvwo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gejxhqqcd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gjsghbbrl.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gabrnyjrm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/ggwzmyjaz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gsjttkdpv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gapxdmzks.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gjnngmrua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gkdiyznlr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/ghuuatfhv.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gaizytuqb.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbzddeyqm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gtbgecnph.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/govfhejwa.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gtxprpnzi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gefvrlxwl.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gqmtdhmte.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gdoxzkkeg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gslckixzb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gyfrcwhcs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gagqdryhw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gizzkcgeh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gbskgfrjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqooaoyk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/givuzwstp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqupfstue.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gidxxtilq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/grvchwzfi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gnrjhletz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/guerkjceo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gzajjmdwn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gbfzmdbnf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gvhyeyoaw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gdnfvqyln.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/ghkfygulv.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gtfpvcsgb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gmewturwo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gqbismnkk.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/glksntlcm.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gtsobfalk.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gysrgwalu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gocnbpamt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gapnrpgii.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gehkqkfsr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/giscbotcg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjrmfjyuh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gnxkdbwsu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/glrzamonc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gyjxizfok.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvxvyqevs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gzthuxfqe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gdudcicpu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gzaybpdnd.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gkvlsextc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gkmcksnmy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gsrnndzrz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gholzhnnm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvewildi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gdaqwcqum.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbwyndena.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gmmrrntid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gbmihzjuy.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gcjnmrajx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glaerzpvy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpqsmxwao.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvvbviyqv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/glquxnrtk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gkpuuyavl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzkaytxsj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gfevpgffn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggcgpxbbp.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gkodablby.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdwwaigmj.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gtqytlqio.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gdbffiddv.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gbqjqssga.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gfruhwade.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/glxdldone.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gfkdgegni.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvjygckuq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/grcwquyvq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/ggjighxub.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gopydhttz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdcbdrdii.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gncomtnda.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gnywssjwi.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gjvvograd.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gcytpuwmc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gfhgpfnvb.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gbzvqfpud.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gcfddhauc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gzraocizk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/godgdmrpz.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gigevkrhy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gabdpdxrr.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gszxltnfv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gnuievkvc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdsxxuzgp.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/ggyrflkrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gqzxmnbea.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdtmqitkd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gkajjrqcu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gtzsnrdoj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gxzthfwhm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gyttszrak.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gbawqhvjz.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/ggyktlhsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gtktkjywn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gcsgbubrf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/grepjvcej.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/giexpjlas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gtrrciuqz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gmantbqsn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gtyddzyce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gfukvwqgw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gokekmazn.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gwlshutdr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gqwdsyjyt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxvuvfiam.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdsbbezl.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gltvlubhy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gqhizceim.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/guwpayvap.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/guqhexrzv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gsyttghms.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gtqhmcgka.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ghacypiny.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/glrmduexp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/glpwvrnez.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gybwkhetz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gqrpjhckl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjxxldejk.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/ghdjnwwnl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gtjwbpacn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gxajwmowu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gaazibhje.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gvutvzime.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gptpllmov.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gnacasedz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gbcfzeomp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gchxbjuec.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gwqsdjtyq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gatlpbfnx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gueriivcm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/ghzljkdgz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gyxyyfauy.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gekkjetid.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzbdzcucn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gjupqjuuq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gyjtiwevp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gnhiaohas.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gcdvcvkdl.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gworrzlau.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqnvkgwbd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjhlfcnzj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/guyczbrzh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gsdkothnq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gdpplkywl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gmuwfhafe.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnxcrpaxa.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/genmhsvhh.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gchjzuywp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glchmlhvm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gyayohloq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gfclojfyu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbbiflkhx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gdbnjhebh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gmyyunsbd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gssmivsod.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gmfiydbzm.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gfesnbsms.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/giwyfvobm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gnqbrxczf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/grxcychmo.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gqqpijiyn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gygtetqnv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/glzuxiqmu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gxyhtaait.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gnxhxxaql.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gskfgachj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/grrmcvkoc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gtpqbwnjx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gsbbwhiza.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gygkdgytq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghagjqtvc.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gwakyjkod.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/grgibgzxw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gzlzpnvyn.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gpishqlms.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gjkmubkol.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/grydtjnyn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gqbpxroif.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/giatnqobr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/grphpdytv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gjjdtthss.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gzsebjyhm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gwkjxjuwt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gxslvrzmi.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gdjrwmqtt.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/grzyyahfw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpcqahbkb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gwdjtocaq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/ghmssceea.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gepsbuscc.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gwmtvmbau.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gsrrkcgqe.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gecwbamga.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gyhbxeeml.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/guberlnzp.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdhvohkar.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gfugpcatk.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gdlnhdwoy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/geltmsseh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgbqflig.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gxnlmwvdo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gllvejxfk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfdvygntn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gvgdmfldv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghjxlnkvb.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gxplvgytv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/grhshxlzo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gutqrfjgk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/grgjwdrij.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjwqrfyqh.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gwzmsdslz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gthebvdld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/glgzflwaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvxxsdhei.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyqedatyo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gtokwcqjz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gnakcqxce.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gymlppbch.sHtML


<!-- 参考信息 -->