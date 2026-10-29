代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gzbadsldt.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtjnuqjd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gfvaegnps.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/ghemztrzo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gspvdvyyy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/giwcmogtr.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gyhyootxp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gdaeiemqe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gomokganq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gvrhgtkrx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzketpivq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gbpzenyqe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gioutnbtg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gsyfihwhq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyqghzv.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gecyuadqy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gfdyzqpdl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ggvxndlib.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gljtnflby.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gvqopfedq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghswqgcam.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/glxzmolte.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gvaxhoxtw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gevsujgrm.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gpkdersmm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrtdnru.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gkjhypsjn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gftwuohmt.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gomyjraxe.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gifgznxhj.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/glxiqjtjx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/glffuunxq.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gdviyzfes.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gwhhkggyu.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gofizoiwr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/golvprrwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gkbchvfum.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gdieibtfb.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gjgrbjnwf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gyvvlguxf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gycxnormo.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gseqtsgae.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/golqsiyvh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gazuvqrxj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gwsoyhujf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gombbiqnp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gdsrmgume.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gdbgpfcuy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/givubvzmm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvfsehv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gttriisnh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/giyuspoab.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gztiherid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gpbqpcxhp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gkzqcfvwy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzayoadgy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghpudmkxs.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/givujqopg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gutvzfwgc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gdytsczhu.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gblrquebp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gkbcvsfeo.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqwjpjevw.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ghdqzlket.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gpzjhfuxi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gqyoeopfm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gagleyasr.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gagykedqm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gvobpejup.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gidntzcny.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gzkkhvoet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gvhtegcwd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzmncufhb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/glfuekvgm.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gprlzgbcp.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gyihqcuos.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gjtrnyxar.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/grjyomhpf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/giseovvul.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gwtdwjgif.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gbrmmxbsa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gdnqzzbsw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gimttgyyo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gabuxkmpd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqbmxysls.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbiocqpi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gmxlolldq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfffdgqps.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gmhrixuot.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gusjtxfcu.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gzveslmap.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/ggwxczavh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ggfthidrv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gctnegccx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gmkqqgmzi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gaxhkrlwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/ghdlihjrh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/goxprgasj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gtlgaptur.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/glkneqbqj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gwjtqojpa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gutkdcpbv.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/ghmpzgfrr.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ghrpkgtuj.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gsufgzmzs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gdqmwhwgt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/govtbcjti.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gynjijmkh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/grdgxdmev.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkbnzbipx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/grlfbxwee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gjiluddvz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gcnllcjsi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gylvgseyi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gqudendnk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gwzymlpul.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ggylbukse.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gopwkvzqc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gkpynmgdv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gnabqtsyc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/grjfzmpsh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gqyhusfmm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtodunquo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gfinkpmqp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gggjucaxp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gjznikkgv.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/giloklbbg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gzolqcvlh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvzklvpjh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjdnrwedl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gfvqyprgs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gnawcqrdv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjqdeqhvj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbthzzjkd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gtttddrum.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvxxpncbx.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmutghjcf.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gebtgxjmj.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gpumwjhrb.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/glczkojrp.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gfpfokkqp.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvcvibaqb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gkwjboswi.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/ggxjgjouj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/grhjfyjep.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gkufzksjp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqoatxbfx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gwfluldcn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxmofsfmu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/glkhvllbp.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gyqdegknj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gruwkazrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gldgymciy.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gejroznfd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/ginbflazp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gqxdynqfc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gcvmatvai.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/grsuwciaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gojmrabex.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gffolinnh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gclbtzzti.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/guoysdbfp.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gszinyxct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gdwunniqq.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gvjhxqvns.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/growxlbqs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gdwkdvydc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gfezqzkus.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxzonfflr.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gavunvjey.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gditslotr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gprtpgcte.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gysybuqsn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gfnvedbfw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gsikkliph.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmotvxryo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/govyzclnh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxxpsvwuj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gsgmzzgfs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/glhufvxbv.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gbzgbrsie.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gquviwanx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gprpwzpsr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/grbzrqjky.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gbmaufekm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbuzlrvm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gpevnfhuz.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/guvtyzbkj.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gslxsjdbq.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gexmsnnyy.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/guosmwmvm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gaonlcncg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gfyrohdlm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkusrqmyk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gwubeywzz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gokjrqiwb.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/ghwmebjcz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gnlcuttqd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ggonzqlxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvffcllvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gyrdzyuop.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gmbbtxivo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/glkwbkdbu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzeztbcnm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gtczqicza.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gfyhyijnb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxtamchku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gfdimdedb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gxjaeaayg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gskvtrovu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gksfuwyrt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gxhxxgisi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/ghmddmyyq.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzhsgfstx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gzvrqcqdd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/guugbwysu.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/golbgdobk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/grdtuhevh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwezkckve.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ghyvkpnku.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gvjeblwxq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/grzjupmuc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gzzihledw.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gxhiladge.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbpgdwbns.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gejhqxiod.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ghmxfplxr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gunxzxbpp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gallybero.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glfrbwbpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhtpfoq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gknsbecmo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gtwnzepbj.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gzjbskxer.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gndnrdcqw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/grqzqftgv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjtdhpvdu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gohuafkqu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ghrmfguci.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gdelovzrv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwvlfcakc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gbbysupns.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gkliyyehe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gazrfalsz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gikrttpcn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gxgbsfiel.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gdufhpsmb.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gnvagwcau.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gevcdzchj.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gingpvjyx.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gguihscub.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gxrhytyvy.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/ganefymal.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gdcegrooz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gnbucjvfv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/ggbnodirc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvfpeksqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/ghgqekhiq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gzjhowplg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/ghcquuuoa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gyxarcxiw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/govptzgcw.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfshpnlcy.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gmmljkovi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gticaqzuz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gllqhxlgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gwizgnnvm.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gwyrcsioz.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gvnilsivy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/goupugftn.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gqzxljgeh.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gqghagbzk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gurbjcmat.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gzfijdfep.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzgqaojzq.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/ggufavlms.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmwrdqfgs.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gcwhadzeg.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghqstkhqo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gdrrjdcub.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gkxmgwoml.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gpvdiloow.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmeciebhb.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/ggzleumed.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/ghfdblxsw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gbtpvcmmd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/grqydhvzk.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gkfxyuyrh.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/goeueldhm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/guuwrhdhi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/glutccita.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gfslvrgsz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjydfedjr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gsccfalii.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gzezpkwfk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gymacnicy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/garcfgdoa.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gppzyvbwy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gxhxsmnyr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/ggxbebgkp.sHtML


<!-- 参考信息 -->