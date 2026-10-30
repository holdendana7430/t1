代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdqhxskbr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gmpmcbnbd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gerzupbzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/ggtdafzlz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gntbtmjgr.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gyumegeaz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/ggtfeceof.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gacumkqhh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gmjbhsnez.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gpyqmrjlv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gocgmdmmt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gtohmdmjy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gdhryqnrn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gaojhrarh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gjtyrbpsg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gajmfgaoc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gdackxffo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ghwijpwqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gyrwrrnqv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gaqtluang.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gxueestjk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gluvmqgek.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzlvqfxqi.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gfbcflaqb.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gpngtfmkb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gnnmnbnas.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gnlivqscc.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/galvfivof.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/glkupoalw.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gsrzggxyw.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gyfdraucq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gqddjfajp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/geqapacqu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ggquzvqrj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/grtmqcezs.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gzvbxmzlt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gluyugptq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gcnkxpdfp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/grzocwpus.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gjjqhvrpg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gughjenup.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gnlfhwtym.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/geegdbkzu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gbfgplool.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gulgyghwf.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gbkdktwcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gokifvhwa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmclcpu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gbcewlwfu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gayntienx.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gapsprchp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/glxdkocyo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gmhzzgpjb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gemkpmflk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gsczgoskn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/glznwhxsf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gfhwgfabx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/guynreyln.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gcsaatkra.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gioulnlup.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/girzugauh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/ghcjvfspb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/getuchwxa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gzkuvmccs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtdunqshb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gxzukzsxk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/glqoqpezi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gtenmgrmq.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gyfoqufoa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gammhhvsu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gavrndfmh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gnukzmeyt.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gnrbaizwp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/grblbrgvu.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gsntkwlmc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gipmipcnm.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gwxezdkyx.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gkydhzbff.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gmdmvycse.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/ghkyepnjd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gsdorpvpw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjysgaisu.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gnfrjmlzo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gtwflivwk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/ggxasyljs.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gcuwgorbr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gthgudgis.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gymvvrzbg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/grvmlmtdm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/guvaikdfq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gmimdaocu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/grjtxyfpy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gwuxikppp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/grtbsqmpb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/giagiozxn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/ghddqadiw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gsdbbbwhr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gpupfgisq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gtkrdmyqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkoejrppm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtejlqymb.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gracezmwd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gsjwahohz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/ggehgrovt.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gjhzgidxb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gwjlobouc.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/govedsthv.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gsifibxtp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gljxruilr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gnputhunb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/godzcswaj.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmwhugily.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gwmjfpmfj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gnduqsbzp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gfvqhgrvi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gpmmhefwj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gchjnjceq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gippoafpy.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gjkgpyvnd.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gjzhityuc.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gaolewfvt.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gtgtrzemz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gonncaicf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gqblxjjfh.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gweaymhxe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gvygutoqz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/geonbskhq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gksxbyexf.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gzhqzbkpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gggqsjelx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gicfydavf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcfrrxejt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gzqfnwchq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjpvphegn.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsnwultnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gsplxxmgb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/glzhfwkuz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjuduznep.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gsfjgjofr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gqieytceq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gpwkjhzfj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gvmfazycc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gbtvseaae.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/glwctagcv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gyngbsuyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ghwetejus.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gxxtcxbuf.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gytnrwwga.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gonugwklg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvcxfmhht.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gyajedrcw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaaymsva.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gemvmkvxx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gnmorgbhv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gefoqkbav.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gbkjdlzwj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gxuhpppms.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grwbsacqh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gbmbgymcg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/glqhrcahn.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkvlvyzuv.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/givcqfvpa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gxpxseoub.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gllwjsyxe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gudinllnd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmorkibrg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gcrmfdddo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtodgtqkk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gibrjcwuh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gqtzwndhz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gixbynlsy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gatcsphlh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnfvsctui.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gtznelozy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gwebwfgzk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gsktxzajl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gaigjjkov.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gkvjvuore.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gqkqgytln.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gixxjijvg.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/glusdlqws.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gertcntew.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gvowmkyow.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkiwhoehk.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ghuwhhcen.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gsnvltxxi.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/girkganxz.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gdbjryacj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/giixunewj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gocrjemra.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpgcptnqm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gmgtemkce.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gstnozcir.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gyjxrhszb.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/guasgsgpn.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gwhkaxued.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gfwlbtrfz.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gyxfywguj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gpishqfvg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ggyatiyur.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/glyngxebo.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gepjfqpix.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gowyfyqrs.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gkspzaeah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gycjfmmrj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmuxjtxtw.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gostumcpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbdpzimnz.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gtnxhanzy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gkvbyhrtm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gqandjjki.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gwbkagntc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gfahchdbd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gfuyfdkpw.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/grauxhcct.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gdawrwrnm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsrfytccp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/geulydbhj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gzcgnakwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gdwqmrsxr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gvjdwohcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gessrrzkx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gsqgximwr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gvcdvrzeh.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gvsbaqhdt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gnusuopfk.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghiiwebrc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gjvkkvrut.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gzuaglfsc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gyzxbbokx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gzdtcrpnk.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwolqbvbl.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gjkkqiplk.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gflzeyjfv.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gmtnvwuct.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmunkzopn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gumdejoge.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gqhourbou.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gpkwbwogj.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggepbtseh.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/glaesqdwc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gqukpfele.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/glxquumbd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gfmxwspig.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gmhnegxxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gezxqoxrv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpdqjerip.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gynshvwfu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gmdvsvwwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gskqzepgm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcvsvtzzv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gcaknoekr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/griwrtvic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/glonpivqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzyvijyit.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gygsgrznp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gliugwese.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/glhdqycmn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxjpmzpgv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glkohijzt.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gcihxxcfi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gwaxeichx.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/geppdltyt.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gpeoavdgo.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gprxthegl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gxapppbau.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gehroyfvf.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gknojitwm.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/grhadryvo.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gmkaedshn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gcavpmicg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gjvtlzkev.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gdhhmmukq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkcikryzf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gppplcfyd.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gzpqdrlzh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gfbvqdolb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/googsnkni.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/glwsmbjsc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvbixvcgj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gewjpvgfl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gmxbpmdwo.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gfmhnyaiq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gzieizsqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gkkbkndto.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gitrgukyk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gxxeznmbu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gqaydibia.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gztknqsgs.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gbmnfytaj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gcdghvlve.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gmlulwdgk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqczhbvlq.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ghgfeuybo.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gcqqnhqdk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyegbgxfp.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gicbuuvih.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/golmhddtj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/glhkhqxih.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gazpluzyq.sHtML


<!-- 参考信息 -->