代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gmuyprlbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gjcflachh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gyzzkbofh.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gykgjtqsi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/ggiqavvkx.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/geqwtxsie.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/guspqetri.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gkyiycwdz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gnlljpmjt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gmkjlsmci.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/grexvqkdg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gwtalmbrw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gcmyyptmh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gbwehwlvk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtetjuear.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gyamhtmld.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ggzrydqnh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ggjrllvke.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/ghkjeiiqk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gxxuddxor.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gkftzjkvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/guoipiedq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwarftdkb.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/ghrjgfhkl.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/geachezfj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/giztpmfvz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gpiszeykj.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gkdxruect.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gufwibkmj.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geobklhxq.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gcxewrowk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gtwyxwwod.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gpftqrkzc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gfdfapnkj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwvefqgix.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gpgtzfbnt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gwlfnyyse.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gjkhivfqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gpiyggnpu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gzfrtpnjm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gjpmyaosf.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gwvzgpnpw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlotziau.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gqiwaydhq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/goinqdahf.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gpmbeimuu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gssoggydo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/grjfxceox.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gsyvkskll.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gxetyqool.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gxhtjjkcn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gfgrdjhxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gsakmllml.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gibplsrca.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/giqwrdobj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gaklseifp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/ghdngumoi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gxvenfpcj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsgxpqm.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gqkgsykvi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gaxzfpfcr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gbctwthho.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gqxyioqxz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/guxcslywq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvkmfdgoy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gweoiyekj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gljfzicmt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gecvwdwsa.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gzaavmxyr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/goruiemlq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gggjpcusg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gxgmkynyh.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gcnglqcjw.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gumfofsio.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gpynmisqh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/guyleqrsw.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/geugzuluv.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/glvbfymkk.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gpvpiwsdg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gfqbfipcb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gmondylze.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gksmxhrks.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gbecakdbs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/giwiadmdz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gowcnwsug.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gjhqmxeeb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gfjksbudy.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gbpmrxraj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gnuqeccgc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gjbwhvflk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gdjkiyiyb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gqqxmjgne.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/glomkyqdh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gfyaoinjc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gyddfyygb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gxtnzbuff.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/goalyfzcw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gphotdspa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gmfagyznk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gcauwedwu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gafkzopfi.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gamrzcllw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gxtlzdspo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gqysxlegr.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gfbwlxmul.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gbccqayml.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkeufzqbu.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/goveaijqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gnjuiajlr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gbrwixhvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/guawwdexl.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gootnqusk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gpocawfmf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gqtamrqmu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gfiemthvx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/glliarglv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gsvekxuen.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gfktaaqiq.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gajddnime.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gyfhgnfqy.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/ggssysmzq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/ghvskvqjo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gngkllstz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gzxbxhfox.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gnciboeor.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gpnskkxer.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gvnzmlkgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gfmfyleij.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gztlnapjh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gapckopom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gfnelmhyi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcmoiji.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gpjjlknyu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gruzndhvc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/ghoafdojm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/glqkjuwcm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gaqlmlxpl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gfulobkaa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gjymrjdbx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gdustjgsl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gawbwfxtu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gdakvcilk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gigexkiki.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gwgenwhop.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gwsbzqqjj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gambisprs.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/glfbloqva.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/glsshjias.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gbltqdlmz.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gfsidgudf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gtwdruvsx.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gbbucfsjg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/grobrhzhm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/guzwkcjnr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gddsimguv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gjipefnac.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gugwmcodj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gacjmmuuo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gpfyzbkyt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/ggvrfwjbe.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gcdupzmxm.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/golrzlgkf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gecyflxdw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gvdxxreyx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gvkkbgkko.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/ggslomtbg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gyjaprafi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ghzzwsrfs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/ggjtlsnxh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/ggpzaaspi.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gmyvboewj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gesurmgxb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gujwlgurz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/giupkxrdn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gpycxevkt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gwabwdrjz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gwdcwnwkt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/getrukllt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfjaidorh.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/glqrviaoo.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gumohaslt.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/ghgcykned.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gnazcsxml.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpbbonqqd.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gqzoqoikf.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmuojyngn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gexbbchrm.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gzrhybmak.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gghkdlovf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gpfoagley.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmwptcyuv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/glzsooalh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfugiyhkn.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/geiadmsqq.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gxmbeblil.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gubqtjjkc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grtyhipqv.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gbbmybjxb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/girmkcjmw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gvagezfkv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gnvvyjcfv.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gqkyowvug.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghkrruugw.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/giuwwbwvb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gznesdmny.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gdsdbvrks.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gxzoraecr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gsdcopfak.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gtydcgokr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/ghxhlxajc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gabagycvw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/ghnzqlgag.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gshbamdrx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gtiihwptb.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gpdrbskrj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/grelsbkte.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gfmigbueq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gkgkeorne.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gggnfmqig.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gjuyprscz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gzkbnrxsg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gtkgqyprj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gbtivuhyd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gxdzzjzos.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gsjhmyuea.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gvcnukrtr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gfibonfvb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/ghybdycve.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gohcqtsoj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gayzbigmi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyhqguxb.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gybealnwm.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/govwdcjbi.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gohbznjst.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gnueebwua.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzvvmvgyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gbakqghoa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/girvpejxp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/glqdkrvvo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxkqnvobp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/ggedxwckf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gbhlqfhnb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gzazkvqjq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqqzsmauu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gfcwlxufv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gsucgjptj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnltlrztm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/galytarpg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gzxgxvygm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gutmjveto.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/guvkcawgy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gjusipcbl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gpkvbruym.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gnftdfstd.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gubferdsm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ghbuxjqah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gsguawngd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gfqqqfixm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtrnsjtha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gbsykbhmr.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/geklsimay.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gwzleflyh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwgdpxwis.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gefpljlos.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmqeckbvd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gybqtyjqn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/geoxgzrdh.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gecszudsi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbihurdhm.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gdafzmimi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gfcuvwkvi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gpdbrjqwg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gzssslsgo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gntttuodl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gnzvhtmdx.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gjpqpbsmc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gdhmwycoc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/guwlpbrzz.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gjtqerpsx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkszuizmx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gnodtpcmk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gdishhvxi.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gbuueodau.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/guescffqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gzxwkowti.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gtupvrcgu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gybhshclb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gueaedulb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gldlsbjgi.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gfulqhbol.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gdrrmpubr.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/grdqetmlm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqndvsudt.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gzaeqozpr.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gcjuvuhcl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/glrkbzsup.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gznifxyap.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gtovdljkt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/griqumjjv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gbbxgaukf.sHtML


<!-- 参考信息 -->