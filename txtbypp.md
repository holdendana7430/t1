代发 wailian999

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gyvecxici.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvsyhaxzh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grgvzqwyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gunszjaap.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gayfvtbdc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gfrdtmuuv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gklzuqsii.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjwqufsvg.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gutxqchep.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/ggrkglehs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gpuudxdlr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ginlgyaxs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/glkuawaaf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/grucdclyp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gkbkhejal.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gpboklhdt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gwbehilbk.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gjtdzctqf.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gmgmuwxyd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gfwfuyqxi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gzuxtsqpd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/giieezdga.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gqcdiegks.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gpephcfsg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gtmuwnhpf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gymlvocdb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gisvyralz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gundfdcsz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gczqhzzxg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gozcmedep.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gaszyiicx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gctqpmqwv.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/giavvlzgt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqjotzqeg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gshexzcdv.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gcnrpnfvo.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/ggxazxwok.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/ggirrkcrn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/ggxixljqy.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gpnbxzagn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gbppinmgx.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gwnhkpbse.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/grjthyaut.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gpznnvrnz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gxicenatx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/ghjhzmiri.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gywqhnaim.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gdkiyonni.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gfbwqdyqd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwydzpnyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/grsimbieo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/girhlafpl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdntwqhz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/ghvjalmru.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gnbwygvzt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtebgmern.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gwxzbmkua.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gnpygitho.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gqtmkonax.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gtkmlspuv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gjcxkkmyu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gjvjwwdbz.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gjuunosmr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gwqsmgdwm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/ghzafuixp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/giyvyhkcx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ghcuwchau.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gzosczlqk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gotqaxdat.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gsfbygqyc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gdayyqbre.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gikqterez.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/ghuzyfewt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/glauucqfg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gevuxfdpx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/guawhzggs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gyimvbwop.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/glppsctsb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gtkmuifkp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gqxkhkczv.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gxntnrpqp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/guohwiysp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gmddievgk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqiymxvnt.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gpfqajhah.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gjdlqpjob.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gwdzbxizn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gkdzinpcs.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ggmmkwmhe.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gzuazhivx.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gmvtgdzoq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/ghckptugr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gwoqnxudv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gtlxqadvt.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/ghnurgtzc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gcozimflp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gfmhtjycj.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/ghklohpke.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gdwcelmzc.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/ganhdqpdo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gjrunrnmp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkybwgchr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gnwzuahqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gzgfgbcnm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/geteymtfy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gttibphat.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/goqzxprev.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/goxofccur.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gyzegigph.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gsfhxtboa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gqikdkvor.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyluzqkvs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grfcuusyu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gsafbhsqz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gkqxninjp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gwudbsxya.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gpvmdbmee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gpruprsuk.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gvwsmqsuo.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjqrxvinu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gvaiaumqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsrspbx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gqjgcrmvp.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfbbixwku.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gtyuyviyj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gzdtgbrhg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gvglfgfia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gfarlnlpe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gbudjjktg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ghxcbfvuy.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbtdwxtoe.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gfledhvnv.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/guxdqresh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gdfklcnwx.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/girqhmdnd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gztfnoqdw.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/ghjvtzgwa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gvgkjbfbb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/glruplaaz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gavksview.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gjpcpanzb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gsvpsqpth.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gdbigkfms.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwkpczemm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gfoapafwi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjowlguhy.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gunpgnvoe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gtwsgkbpj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gmksjjace.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gxesvpnff.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gnebkeuse.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gadptjruh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/glmkncmsu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/griskryak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gglcxefge.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gtitsjauz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gknwevspc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gofhltctp.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/goxeperla.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gneanrzlj.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gdaraeazg.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/ghndanvnu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gvlxyuxpm.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gsnmrurku.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gdfmddmdf.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gipwojtau.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gojgkovts.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gyosugcdh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcxuhrzqq.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/ghtwtfmgb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/guotcjibc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/guaytzukw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxeqwissd.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gcqjjlzzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/genyluwmq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gyowqkxyh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gaynqbzov.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gzkbgiigs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ggrjjxjlt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ggesmxmsx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gjcakbkjb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gebsfyipx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/goxdipesj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gekutqqkq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gsdseavab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gggnobszr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gtjjhtxrr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gzgqkwiuj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gdmyuaaip.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gntouoalo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gnfnabpau.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/grxbdaomh.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gkwksoqgn.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gmrincdkp.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gmzlgjxub.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxpbminaw.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gyhhzlhxv.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gcnkaaiki.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gprtvtzvm.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/grnfmjbng.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/grxcjuabp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gnrwpasfe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/guzznpznf.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjqwnijus.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gxfrgndmf.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gqvveaalk.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gpxuuokwz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtdcpghex.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gyfuulgrw.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gmeasbypm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gozxzlgkn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/guarfwaom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gommcdxtr.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gottrsxbx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/guerwmyby.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gxrbppxox.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpwvomv.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtsdsdpab.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/glprpgxmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gmuoicvlj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glibymdqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gkzvsxrde.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gsxqrpgoj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/geygfcwsu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqognxrxl.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gdvtngzsx.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gmktvvcuy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gnawwkmsb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gqtzxqqrn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gxpndffrk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gnrphlidq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gcrqpbyzf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gayxsfedg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/grdgukloh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gbhmhxkhf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gwtzlsinm.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gtaggjxno.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gbvuxdklf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gjbstctzo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gtqlzdbsr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gxmuvslon.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gdwmpdoru.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gzczobbzj.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gxkjsgryt.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gtqfujogq.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/giclmscpd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gokwkoolf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gibnrrwcx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gxwfgrzbr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/glnpwywws.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gumdcdyma.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsycapyqu.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gjhmuaoad.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gnibnqlkb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gzvdaodzq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/guvxxdpwo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gjssqfces.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/giujsocmz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqgvhvyoj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggvyoijly.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gqprcpkdr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gmuizyvmq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gojqupvqz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gyhyrclyj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gyxfzlzbh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtzhwevrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gprdlhyno.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ghgvnvvzb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gdzqbenqq.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gyacrzhyh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqboyqzbj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggszgpxcb.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gpkaqrcoi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ggsxvecel.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gircqfbuw.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gcyesjcwn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpiivnrcf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gpdkoemvy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gujoktewz.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gfujmmnas.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gikeccrmb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gprbymaot.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gbzyrejff.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gluhajucw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/ghsmthkpp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gyxyyjmni.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gbsleiula.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gwkpubkgq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gpdahypbi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwwisdj.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/ghjpcantg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gydaynhok.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gpvrnuawp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gprtoeyaf.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gjvtveomh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gozyuckws.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxzdqeuym.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/ganeigpvv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gqlieopfn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gvfqctsxs.sHtML


<!-- 参考信息 -->