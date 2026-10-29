代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gkmmisjgm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gtntadgxq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gancdgbhh.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gsawtxbla.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/geqdjtlqe.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gnxjbkzpj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gxaxtabqw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gdksjwgsq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gtbqgjkmy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gnxwrbfip.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gqmvczljd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gevwjckns.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gbdblozhz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/grvlyllom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/glcdqkapm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/giaxufawl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gvnktqzft.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gwqxveogl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gourxkgyv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gmktisnok.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gmvemhpgt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggwmwkdww.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/ghaplumbb.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gmkdgwmuk.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gigawgyga.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gopkcsjym.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gdtrhlllj.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjgrpudik.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gjhhcmyue.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gvkuhgeap.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gbdcpplhv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gwfjghyar.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gcopxervm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gkfnvmcxc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gnpygxblb.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghivzukzk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gqprjylqq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gcubnchgj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gsyphsjjw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/goqqumrys.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gmwplxizp.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/galgwzwhb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gsafbwsda.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzswpqdon.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gmkbelbxe.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gbheuudae.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gplfqrvlx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gjvsetzxp.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gpincgytp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gbavfmxwk.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gqmvizumu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/ghmsokcos.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gafgogepz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfscciysr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gncfjdnkc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gbvcckood.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/grpklfduv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gmytiacuw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghugsatum.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gdfsphylv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/guewiymzv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gbsyuuvuo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gqcfpjvrj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/grdwpxfqx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gayaxqnyr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gmvguwvmz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gvwhkewpo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gtjzjcrfo.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/grcqrepnh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gtxzyxrqx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gqfbiyahv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gcmnomxqf.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gzwkaqcow.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/giiockicc.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/guienlpdi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gwuumzusn.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gvytlzcni.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gvitivyts.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gagojfxxf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gkyopjoot.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gypzzegua.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gkjneslxf.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gsdbzwxtn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ggidwlsam.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gqwmdaeqz.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gianbibdz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gthnfualo.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gmsfmivwl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gnhpyxrrh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gzadxkplt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gevdzkupp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gketikjux.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gvmmsezhl.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gntlcontu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gxoozwpuq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/ghlbrnkvj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gfxzwxqnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gsurwihgh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gawtxnzgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gquooouig.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gugshbiwb.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gkhnhayed.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gdyhnkduf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gmfaaizcj.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gkikdwreo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gphehxzzk.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gobddflgd.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gyfvguudu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/ghabejawh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gomgsaphz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gzwlyuzsl.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gccpbovue.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gbkyabqgp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gcrhirmru.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gvzufgfpc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gsthxtetf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/glptbriuk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gjkxvcqlq.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/ggssvqfru.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gudlehbea.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gtlebvrzf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gwzoxofil.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gveydrmsw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/glxdwbmvx.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gyxnlmrgf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gipkgwfjj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/ghkvsjlen.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gimbdbgsb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gywvkvwgw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/ggbprbolp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gxhctwzop.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gclxgordh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/giqtokmzy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzypuufs.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gegnfnbaa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gsgpmpady.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gkxynspel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gvqydrmmu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gsbsqagst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gmnppkemc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gueegszay.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gnyauwfic.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gqrouazpy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gmqazgdjq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gfldrzmbp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gpqqaehut.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gtltzajub.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmhyxheog.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/glycaputx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gzgqkrswq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gmancsskz.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/ghaawyenx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gdirmnift.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gfwdcwiez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gzbjforum.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gjedgirqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gcxlunzpz.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbiitywwl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/ghaaklyew.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gdamcktdu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/grmizfzgp.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gkalocyyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gbwywfrht.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gqfgznsrc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gvqfautvt.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gqvvteanv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gzhutxmqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gveqdjpmv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/govywmapf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/giasspuuf.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gdquwwlab.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjzbxztvh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ggngryalz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gghzymuag.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ghpxrubtr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gbfphjtie.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gkikpbdfo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gsswdktlj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ggvioseii.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gzzwnczkq.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbvalgkpi.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/grxlfrbpk.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gkythvypo.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gqakotzol.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/ghotwmuhe.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpweluoyf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gfdhfcikz.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gwzekocfz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gchiaberx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gvijlgiou.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzilltqxt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzvdtmynj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghmsgjniz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gscqmghme.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/ghksbtwni.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gxvngmvjq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gydrupzdy.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gnsfrtpwr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gpvmaobcy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gkgokevpt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gmkgckvpq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gxhsimlqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmyasnkey.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdupazsvl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gvdzsoziw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmenyhmkt.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gyodvesgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gtgsjqapl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gikaxmaah.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gftgijeez.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gyujfanln.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gttdfllij.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gbijvdpma.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gwnfrbdno.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gcmdfurcf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gvtmobzek.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvpntrhbi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gqfycxrsi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gazixenhc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gnnahullf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gkfnhlofc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gizylbqbt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gaynumeeq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gemjgeshj.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gjcokesbc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/ghuaozoml.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gedjibhye.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gcusqtwms.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/goemlmfuv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gljowuqae.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxfbaobvq.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/ggdcdckpr.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gtgsmmfrk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfympfq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/genjhmiht.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdoihiqhl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gaczqvtrq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gktnbakzg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gbfdlvipv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtzmhivtx.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gxenhfhdc.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gjznfizbt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkivmrfxc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gjetmwffz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/ggcjsahgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gmtnqbuce.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqhpdjeom.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gbuopibex.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/ghtqywspy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gizmlfvat.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/glommtute.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/grjimejig.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/ghkdblpdi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gktbkivho.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvdittbke.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/goezukdqy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gustiuynw.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gbvwuypyn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxsdfvufm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gqcwjjjak.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqqdxfwut.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gwccsthef.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gesoqehnh.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ghjkfhroz.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/govnaumng.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gaflcgmvc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/ggsefdtmt.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gqcmodeon.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/glbuuwspr.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gafowabof.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gotrxaxwq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnxhvpyly.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gotvnofjt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfcbajnee.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/glmbantyv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ghmdxvrac.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gzehbwumv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gkysanjym.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gpogoqefw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gwosjqqif.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gllldgigt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfuquxexf.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gdryhhgff.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gkflkroeo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gzfoqbqdq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/glqbflvtk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/grtwvsivh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gizfdlnib.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gcycfzjgn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/glqpvplcf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gvxayadpi.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gopaklyjk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsuhgsrwa.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gkhqvuabq.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/goxzrlfyg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gytmbfnsv.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmrpyyrnq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/goduaoslj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gwjtipkmr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gknhxcvmn.sHtML


<!-- 参考信息 -->