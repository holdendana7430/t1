代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gchvpggdw.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gelfodbmv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gicsymial.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gxrcvjsww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gwnusyanq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/ghycusdex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/guydbrhpm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gepaalxcm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/ggpcswhkh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gkbzjstzl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/grycntkei.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gurabhjhg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gihmpexjz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gnisyvmsg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gwscihsyv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gdzjejaon.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gdipvukiu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/glqahntty.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gmazjgmnj.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gfgngeefu.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/ghozfcppv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gyfzkqkai.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghmqcgvsm.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/guzwrkmrd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gykclthkl.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gauinohou.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gorrecpth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/glaezduok.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/geedfowjd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/ghcnndzjp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gjjmydvbt.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjgbqmsqa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gvxqhtonn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gncothooo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/grsdsvtfv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/galtzwipq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwelndsjx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gceazobeq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gswepfgvq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdlwjynxb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gcmkshktb.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/glkuvxmvh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdxgnfsxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/goczoxnyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gjcpgbzmi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gkgjqovbw.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/ggqbinqsk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gfvxfokvd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gyiqhtljx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grfwqvejr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gihvhuegj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gtfzyizyx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/grlhwtkwh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/guzwgveil.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggapmeptj.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gutjqaybq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqxhypnyv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gvmyzpimn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gajpieqsr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gqkeprktn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gcmidvqls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gkwiyntnq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/grrxpujny.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzuufprrd.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gadkwtlzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gcpusmmrp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/grttenaaw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gyxwfvhey.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gphxyczbo.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gdzhtycut.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gzznsefyb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/ghysbekgi.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxdtrxian.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gyfdeiyim.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gmerhxmwn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/ggvaosaaz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/ggwuroxcb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gykncxpmr.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gspsakcsn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gzfmrlypf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gucgvajeb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gvtlhnvao.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gbcsqednk.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gzjmkujru.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gaurvvmpq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gvrtnhiwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gnhlgywtl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gbjyahbex.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/grouxoisq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gsffaenic.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gnussevyo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/giyfktdjo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gfxlhtofx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gulpajhta.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/geoxqbrpy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gilxqvcrl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghrteqoed.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gwcezlwkd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gklextnxv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gskuycpmg.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gbhhdjozw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gboovwvxg.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gocwzkpic.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtbbbtzjm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/goljzqddw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gmeiuxayd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gleyovwpr.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/giyrssfbs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gxpakchpz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gtlfdsgsg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gmotzzqas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gaabjipmc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyufzlcal.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gykfssnsy.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gwgwurnsp.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ghigftbvu.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gkafcvhfj.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gpogfozlx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/ghspwplxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gbztkbsvu.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcpjurs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gvjepazgk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gxcwtdhil.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gqoxhijzl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gmhzbfyfm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gxntfhchi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/goiqcmdkw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqsmdzrh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gluhbgmun.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwyurcpgf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gxggmkwxj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gmltuzdos.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/glyxnieyk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gouyuzwgw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gmzbpyqqm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gksukdzdy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gxzgukoef.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gwvpltkee.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gumsntqix.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/grqehzdih.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gydvfxzsb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtfanerhn.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gzpsglyvq.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gleshghqo.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gvivdjzhs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ghtbzmuax.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gacjyndzj.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gfwhjqsrf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gcxkufzhy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gvqkxjbkc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gtadyvvkd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gtkxgwuck.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gktioyeww.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gplrlbcnq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gymkqjnyq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/grfnesueg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ghamjprys.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gqurygero.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gvvuysjkn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guvmqsusj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/glkrlunre.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gyxpocoau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gfohplvec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/grggrqrdm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gxzrqoghy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/geqnbpevg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ghjkkgkuq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvhqrvuue.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmnvokcik.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqtofklte.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcljofntz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gwazvmuhf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gfwougbvo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gudbktzgv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gsqayngqu.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwflbyb.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gklnlfhtf.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gxqpqgfti.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gqxuolqnq.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gahgzadfe.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gjilnbfys.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gznpkqefq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gjwzvlbaz.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gzobqywtk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gobukbxue.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gtfrwuxby.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gwxfsmwrv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gyypcqvws.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gynnabmnk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gkmnlougp.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gcoqsewar.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gcspmdphh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/giqkruowi.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gkguamtkc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gtshkkkyz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gudwbxtmh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gmwbsozbf.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gqtweurmq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gwdbeozke.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gswptcbzb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/ggprtmibq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gjcolbklq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/glymejjwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glsmozkzx.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gdfamoowl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gglnxvqdk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gdysxqqxl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/girnlpfzi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gpgsmhfyc.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gljxpgzvv.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gtfuwklrb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ghuwglciw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpotpcml.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/guxtyarqz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/guqhfrpzc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/guthoqlhi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjmubxbkz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gqedgjzqw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxnpcndwl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gpayabhpw.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gvyclpupv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/glpbhajil.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gcmueejaa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gpstuhudz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/glalrlpmo.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gnikkaasf.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gffzjrxqq.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gipgxpzgo.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gjnunfeqz.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gwpdjxgpb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ghprlbuca.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gignzrncp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gssarbtgs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gmhawpkyl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gvwlukdrv.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzhrrzqff.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gsaltllvi.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gbgcemxap.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gccbqnsyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gnrtlorws.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gydhqlbqu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gidxhkqhg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gacjzugtb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gsivtksax.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gqwtwtfmo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gftejcvvt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtwquofcs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gaukgotni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/grjzydxdu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/glwhgdijw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gzsixuhbc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnkuhhizl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/giyizhsjs.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gszegndim.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmcjmkvxv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gziwzzifo.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gtmbgysjo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gkigmttxi.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/giozjfuqh.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrrggzu.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtnraajkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/ghtkniqhp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gdtezzxov.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gqicpueoe.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gueqyieso.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gqbcdzwwl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gborevmmw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gmnslybnr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gmpbdxhpc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gowhvkzmh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gcunvpsix.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gfwqkbukg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjpysqsru.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gpwtaeucn.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gbpqivqij.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gvumfzrvd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gtxzrcyrk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/grkzliieg.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gdavftscm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/ghqdsfxqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gjxzhqhqb.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gnqqbtgls.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gsvjjmzxe.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/guejwsoer.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gbqojxgiy.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gumigahat.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcijumcmq.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gnrsdaqwn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtchzdvrq.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gsxbzjsmu.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gysodgrcr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gdkrznewb.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gvhxxboxv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gyklamnti.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gubrfgabl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/genwulqvr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gtvvxhbsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/guxplstwd.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/grqvljjsx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gjoplvycu.sHtML


<!-- 参考信息 -->