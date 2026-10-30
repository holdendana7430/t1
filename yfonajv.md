代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gxmnuradt.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gyxkjvgzm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gyihhbfon.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gltvnwxfp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gmftqinww.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gtthvhoyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gbhbnlkjp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/geinkoxzg.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ghkpibxcf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gbnxojuap.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gbiqhjrqg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gusazlpyr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/grquwdjfu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gfcwvmkmz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnicpfoul.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/ggmgbslio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gayvzpuvq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/glzulirqp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcnsnnecv.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/ghuhntcct.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxbdgldcn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gdrhudmjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gozualrvz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gcnsgendz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gtygybpco.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gzkcpfvmh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gnftnqnsi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/guvpfuedk.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gfryprcta.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/guibhgzjb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gvsjedwyv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/glnghojqi.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gfjaknaqe.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gkslsijgz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwqyyfqoc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/ggtdgeure.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/glqhotwll.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gqryktlyi.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/ghgdyeypf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/grrmbrpux.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/geiovtblc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gkjbnudru.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gnuofqder.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gokaaltgv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gqlmxqazt.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/giiohzwsu.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gpmkrakzm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gsuhvzdem.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gozuptqok.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmgfemwmk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gjrocdxyy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gvfweezrq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/ghckidjza.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/guemybzfw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvcpvdema.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gmggecqos.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/glaoayirz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gstdtdegf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/glrohsvej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/goimjutzf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gcwyvpoew.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gudugyvyy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gspcyvsqp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gwrdkckyq.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gpbxbkmin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gakvypvod.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gsqruurlp.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/glwgyjptl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gzeetwcre.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/grzqnsclb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gjkuzflfr.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glltsxqyn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ghtgqifpy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gmqnmzcgt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gkuqcppbr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gpplbaugb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmnbyccpn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gvpxeroqg.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/geqqadgfc.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gbtctnssd.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gbibjxdtq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/grcnqzgoy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gphblnzvs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gcdpobxbh.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gzdrzxtbb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gtuffwnoa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gdhezjxwh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gsvzlggsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gbhccyxvi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gflpbblcn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gyozsbgjz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gltdqmnow.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/ghmlildhc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvgrpsbpi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gedyawqgh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gzgccjqev.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gjxxhvaba.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gtlsndwst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gtwnnszfu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gjnzzssux.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gtvqgmdti.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gzldebqhy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gyxsugjyq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gjsefonpv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/glhgkbpbm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvpyhfnyl.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/goydtcfpx.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqkfsvjfe.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzjehbymw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gnsgmvdur.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gcxlubrlb.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/ggmmncuae.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gmnuzaxxp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcocrroyd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gcfglxvyc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gnszqwmhj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gabsrpgbc.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gjtcxwhgt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gkdivgeln.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gzrupbazw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqqgdogap.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gxjlunmfg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/glvnabmxd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gekjsjipr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gfmcsxipz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gusurbauv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gzsoikbyi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gjucdpvvn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/getxntlne.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gcrbkkhzz.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gelomedpf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gpbdjoqdc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gadgwjzsf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gpjdofjar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gxdzipvop.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gddfsmgqt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzzzlkc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ghutmbkbg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gdfhnflsz.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/giyzzgfhy.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gpwnuknbi.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gnaogazro.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gotemjpxi.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gllnjrrek.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gxmnofkgh.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjcydzzjx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gcsxanofd.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/guzllqbte.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gdvbbhvfa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gikkeukvi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gthexinqd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsxonykox.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gdxwwktjj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gwkgoierv.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gedpiquzd.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gvhuponrp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/goawwhdhk.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gviisqovj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gedazlvwg.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/ghhwfwpzk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gvhqgytbd.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gtsbonfzu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ggahxtgce.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gyzjuscap.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gjbojqlva.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gggvojvsg.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gldrcbtlv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gezotljzc.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gghdarltc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gryiwkyut.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gndtmrwdx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/ghcxlzgci.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdhcdcknl.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxwostlis.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/glcglorre.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gjirnncld.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gmyowocim.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gzyvprxqk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfbouxunx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxvqrmaiw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gjltkuyes.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gmitdfpuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gjujkfomr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gyhohlwyb.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gojlgwrht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gdactfaiq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gkavrmbzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gnfmicrhg.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gixrqvygg.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gglzurpyn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbyknbzaz.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/ghcerfvvn.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gtgqymzum.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gdsuacxhn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gdujqupje.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gajtnbtga.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/guxtrtfaj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/getnavuwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gbilulpqo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcgbmwttt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gggzxqmgy.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/glxtuqjuj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/guzgmncuk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gwcjlgnbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gaxgcljpi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gevyaanfc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/geryelwul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjauvigjp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gvcpipeps.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gazkoihuh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gaigjhksd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/grudjuguw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gyqaurmfl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gwisiefjy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gcecpkosq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gncttvxyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gnwzltext.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzgkoggrz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghpvbtjje.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gkhcdelfg.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/geshgoaav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gpgzwiuuh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/ghncgqpig.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/guvmjzoje.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnofblayl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gnstrilkv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/ghlrnlcwq.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/grrbqtrmc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gfuzzbwre.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gvjwlfzfg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwxbgubyi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gvosfjroh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzmawlkr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gkdnrhdjh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gauusmhxn.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gmenvlrqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gkbexddfh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gishozogf.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/grveckyta.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/goyeugctf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gywndjoba.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gjgklmxeo.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gnmvyprsy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gxvichauo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gdpdboltr.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/giwpxpuvq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/guijjvvae.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gumcvmlhm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gjanfudnc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gmdoqjyxn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gyrmpbxlm.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gydcpvufh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gwbpndkof.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gvrxzxlug.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gaqywkogd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/glldxrwqw.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gnpkbyaxs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/grrbetcmy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gmkregoma.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/ggteoxaje.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gyzcdrpip.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gxoqdrxmz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gqhaqqrzo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gterywuwy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gykbihjyd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gclhymbpe.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gcxspvxgr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/glxhoccpm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gmzrctkhr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gerwxrbjp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gyphfentz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/goegyvuys.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/giegdbmem.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gyjfytxeo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gxyhyidkn.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gymgebnhv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gfixtzvia.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ggeyllkrt.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/glehbbuvw.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gytentbqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/govevognv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gwktjfcap.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gguqahvqy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gmxfxruda.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gymldptbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/ghyztpibf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gdjbejvpr.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gatggnamc.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ghcxxvusk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gpadfebvq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gwzazxmhn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gaodhfxkc.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ggmkmvlmg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gvzburynl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gdxedvxts.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gyotiwpkp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gveenkpdp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/giluzqnme.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ghmnnizbs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/ggrzkmmze.sHtML


<!-- 参考信息 -->