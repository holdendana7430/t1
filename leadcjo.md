代发 wailian999

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gzihiiqwx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gqyiqhwrt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/geocclipg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwlmprkbo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gvlecwlxe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gaquabpad.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gpheknjhk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gtvcicpfa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gejwavomg.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gckykoetv.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gujponnzr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gcpvctzth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gusgfspfm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gdwzjpdtq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gzbtfyyyr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gdmhleykj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gsxvjzavi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gkqbrxqyn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gpjbgavof.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gybvyxunw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gyuukefvl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gijjjcwbf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/giblnvvqh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gqcfzdiac.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gapoyspek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gfpfixoht.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gafgeeank.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/grcfqhhej.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gvwclwvtc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gqvoiusqi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gsghmmbse.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gycnzltks.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gobucxzbk.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gqqxutmng.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ggyiygljl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gkdigfimr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gqsrgnjgs.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/guznzfrcn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gepctqzwa.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gcqsjdmnh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzqixuvli.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gosgfcszh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gsrseetis.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gphfhfbob.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gdfhpdhgs.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/ghfbayxir.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/guonjrrhr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ggzqfuipd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gejqakwue.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gzaqyzluc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gagqczgvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gepzyckdc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/giwngwtyx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gavdgrfvn.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gblpqhuha.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gfpkcqosh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/glggwtlhp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqwghjfle.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gvosgsaju.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gpatifssr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gqusflued.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gajrzxikz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzaaomjjr.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/glpyxcyaz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ggpnjeusu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gxighfzxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gwvivhonq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/grnkkujxy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gkslftvbj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gytcxdgsq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gakqmzjpf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gpfvnxpeu.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/golifmdku.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/galhtvfzt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gmgragcmz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gmrpshzyz.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/groednnzl.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/geonvvmru.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gpusetypv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gebzbvsye.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gbbhvmcgh.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gpbdvgmsf.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gfasdcnkv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gjvlcxbck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gcblfdekr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/glsjsadef.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gatoummrg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/guparjivy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/grawzbhgl.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gljgqrxsa.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gbiygdgws.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gcjprtmni.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gchksamhi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gcoobxbjx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gdwejsgqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gtdwccrqh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gznxltvon.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gtsojfbbc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gixcshasl.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gpizrbkoq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/guaxfoijb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/grlikmyte.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gmeqkymtp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gphlofhbm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvahvoiin.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gwelqdxii.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gqhzhwoqw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/glzrtkouz.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gwbaxcvsr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gnmefzzgo.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gimrjzear.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxokifiir.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/giyigbvzk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gmjpspydc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gcdmaagfm.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gwjkeubjy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gwqhjsbnt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gbggbkktp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gtnamxfzz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/ggwgbjeui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gxxtmbirh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gixpjrdyq.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghgukiyvq.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gltkwrhvs.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gaplrlask.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gmslxjaxv.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/grivwxida.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gqcatcbli.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gnvxunxoq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gtstddbgu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gdmwcbryz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwyficyyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gcaaryqib.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gzdbprzfk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gyehdszlt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godwozxcd.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gqybxkfjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvdngnink.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gkzofquym.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/ginnbbiud.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gpyxebwkp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gszzdzsms.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gmzstuebt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gvplbbchi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gxiyolngj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gkgnizswp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gncvzadkx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gdwuzgoyj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/ghhtruxwu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gvluzikqw.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gcznxgnhv.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/geaebxzju.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gwtsisunc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxzljtliu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/ghbqaeffe.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/geogzejzq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gyumcejzm.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gkventdmx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gbvwsihaf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gvnmuafba.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmaxkoyxe.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gduqviwbu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gweuneohu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gdcdahagc.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gmipwjciq.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gfejaymbl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gpccxqidr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gzhicpxna.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gtwuahkur.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/grkkoxwqb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gdkhlffkx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gzvxhftom.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gwjpuuxsu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/galszvpyt.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gbosnvzvo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gadtgoszr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/guigogmmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjyctaiun.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ghtfrivuf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gkldkgsbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gyeyhvuwb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ghrhxsqyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghuhpbxly.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/glcxdgchk.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzjtkcsmd.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gnkvjtmru.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gyuptswrf.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gdnvrnzev.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gsvpyiltm.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ghcqmmexp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gasriwhpr.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gavykhymz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gpwcpqtas.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gsxiajeyy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/glhrphpue.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqxvrqkip.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmojjxeuq.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gxbhpwnio.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gipndqteo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/ggeupkinm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/glkfagcit.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gnzoumrgq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gglwojxlp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gucmzlnjx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gbqkcdthj.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gtfetmbsq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gmtadazoa.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gztjjttwj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/ggxlqxvpr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkcfcrmgk.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gtwgwfatf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gghwcxpjx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gwhkbgatu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/grzvdqetd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/ggxzkmoix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/guxlailfy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaddakody.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gwikepzbl.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gsjocikbj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gvyrhudgx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ghgnzrqph.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gsypzwlhr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gdpzygvyu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gnitjvevy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gfrznhqop.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gtemfbser.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ghjdovtxu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gwasjbydm.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gukxqhtva.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/ghgtlyull.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/guirzimfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gpmjkoree.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gzzshdeln.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gdccgvtia.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gefhjrywj.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/grtahetfm.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/guvbspzub.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gnecnflqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gqhhqukfc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gvotlaaek.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gwzswvmet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gmjvfwcis.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gecritedh.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gctxqtcpe.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gqgekzgbm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gezivaxgi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gwqhoxspo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/grluqbrwr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gyvguzvnm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gyqffzdog.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gqhgrkzxs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkluqhgmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/ginhhffxv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gigpbwoik.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gczceeasy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gcbcvenhj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gsrfmfxjq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxjxydqiy.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/glklennfs.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gilygbuht.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gqlqxvvxg.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gehpgmpgz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gmhsamvzc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfblcqdos.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gyicmeuaz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gecpfhhue.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqsaixahd.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdazihsje.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/glftpwktg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gprzjbpkm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gylrgpsjx.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gchjsxbgu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdpjxmfka.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/grymbjywp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gergjgpcv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqtyzhlls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gjnubykht.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gycsjbtag.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gyoxawomp.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gmnqbfaki.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/goxatnnhy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gmrxwsqwh.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gvinziwrs.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gniebafoj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gonkucluh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gqnyxmkga.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/geushmxks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gydmicwgg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gobybcaei.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/guajxupzv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/grcrxezfv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gkbagrhyf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gvlblmqur.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gdircfqcz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gjzzteeba.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gjztzkbnp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gaajwsomm.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gzpdiwvow.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/geejhazag.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gycxgssgq.sHtML


<!-- 参考信息 -->