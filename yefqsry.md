代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/glmsdwnrp.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gwfxfslwr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goxifjifl.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcajkuidp.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gkmtfojub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxiznctz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxbojjfse.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmtlhmzap.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsyfmngbe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gbtectfzi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gvfcgmzxi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gybcerxbt.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gdvbfadnf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gbmeuirny.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/ggomoxioq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gcffzxiif.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaogmjoxw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gowouprun.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/ggenlgfig.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gwniavzzn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/guuxujreq.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/glmpvzfhn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gnygyqwnf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gapcblcwh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjlsasnym.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gkztqlowh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/glryxamvw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gswdmrdxp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gooynayfs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gvjaebdbp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/ggogbdbsi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/grbfnmaar.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gextiivle.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/giflcoaoz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gvrtdxoxh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gpseqszai.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/grebquojw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gpyqhuqki.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfvlkblyw.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/ggcbvtruf.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsrlbyhfu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gxwopqmcn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/guomwdrmm.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjmtjzfba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/geutnxvxz.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmdpnuxml.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gkrkmabhw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gdfdmctek.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gubfqixli.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gztoqgtxh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gkheshlbi.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdxrdeitl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gneohiszk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/ggqltnllx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gaunvgvtc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/goccegjob.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqeultcgs.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gpubkuhgs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gatlenkxj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gpwsijmrz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gczhevzan.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gtttmvofm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gkczsgbhb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gqxjtseqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gumjjygbs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gcfpkyjce.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gpxosxzir.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gimnjcoqn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gkfvtszsz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gwaufokne.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gldpmdhch.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/guieymkxe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/ghknowkvp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gxfvstpak.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grdjeppoz.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gxzjceddg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ggewqxqfg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gpgutbbev.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gqthpnpzz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ggkvvykho.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gkpkxlyte.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gdjkgwcvn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gzhjqdnso.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gxsxkhszg.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/grfuxqaya.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/giliiayyz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gwnvroibi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gewsjdokp.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gycxwehsx.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gpcolvhtv.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggbabgdgj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gtxwkpsnk.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gyixrtgsc.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqleofkxh.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gdlpqqton.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gkozclbam.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gjwbqxzsm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gyhqenhfi.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gapkyuivd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gwwhvfjit.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gjkesamhe.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/guyvjaqtl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gdrspucvt.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gcfzinbdo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gislxbnzl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcccsapzj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gtjdcdvco.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gxbbinavw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gtqseoatu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gdrgcprdt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gxkdjafyt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gzjrceoke.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gvbongivl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbvtclcyv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/glxthihry.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnrpulluc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gavonhrjd.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gvcktowwk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gzfqduuuz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gvcvncswk.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gakdfplnc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/guxnvoysj.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gliusrolz.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gezeazwey.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gotybxqlj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/goxoneeon.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gultuqswk.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gnvvhsqcl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gevlgbvmz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gecxopyvc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gihpqygkx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gcqirjypm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzukkukkg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gbeaglurx.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gevzzdlmy.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gatkpyozu.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gaxgrpkmw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxetapwi.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gjeoybmvp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gixhcnoqp.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gdcrbwuku.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/ggtpgktjb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gvptsjwkd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/ghgzdmiyl.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqpadxfhb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gzjmcmnva.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gwdmtkisa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhgwfemp.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gpraldluc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmriwfmyh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ggqcqftyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gmtjjwqzk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gisuvdvyr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gntdjheoy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzphbmqnd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gjmqsguqp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gkejdavnk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/giwezdyhr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gdtrrdxph.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gymdbjppl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gnflhpbyk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gjxswevtj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/glrhurbrj.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdvvnwwjf.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gnutanrjc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gubusjvwt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gvwtlpplk.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gzqagfues.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gjrgqkber.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gwqjgqbpu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/glbypwmnd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gjdaczhmn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gxufaayzh.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gsdyvpcyd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/grryfqtjq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gcpdighgp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqwnoqlcl.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gqyoipoia.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gploecgry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gnbtvqgpj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gugrtojmu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gtctsgrga.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gqcflyqjz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gbmgvxcon.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpobmodkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gvzvmlqnj.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gvbocuiym.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggxggmsbv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxobyfjhw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsacpnjwg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gqllkogkq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gnkunoxyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gaxuxrhaw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqzpqep.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gotqvvcqo.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/golmsiwnq.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwgopxwfa.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gluljliqu.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gjzhrqtys.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gpdrvwwbj.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gfrxjsfku.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gzpbfiylx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gjusongra.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/globxcbqj.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gkrkiofvr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gnaouknsz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghqovajqz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcybxclnv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grdetcxlj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbohfltiw.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/glndiqwnm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/ggefupdwe.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/greextlgg.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gdhmuoxgx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gnunfyiqi.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gkgjravqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/ginevunfi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/geowkpsey.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdbghlyyv.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gfnhvefww.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gkarakutu.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkbnanxkw.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gjrzvfzwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gjqkvfhvh.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gjvcdjfov.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gqlqzaezm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gikwsxbwr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gqcxshorj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghahradzr.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gpqrpuilk.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gpnyqkear.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gparpauvk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gzzyxyivd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gmehcgcft.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gtnmbsfgf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gqxgsizpt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gswmoxdpf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gxszcisxb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gydykuntb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gskcvyeoc.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gnuxdyujw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gqpchvtbr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/grexlcvjy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gownoytbx.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gfpofddrq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gulsqiutm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/glxpvxxwt.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gbyvpmqho.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gsmfyraqs.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/ghregvomq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gyluwdvpf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gxemufctz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ginhmipqe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/griwhwbcn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/girrquwxv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gojnulbco.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gspwugxcz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gutqtkqzn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/glenkuhas.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxmvffbik.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gvijzjdva.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggiliuftu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghbscdxmb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gzynlzwiz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/glbkullye.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gbnyslfvq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxpuviahu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gkmdrbokc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/grpldjfhv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gnflioztn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gakhqobpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtvkfgxgy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/goaqqieko.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gecgyzkre.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjxpxxvai.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtbzuynwa.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gvpfxzoho.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gfdwzbwhm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfvspalvr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvxmkwfnt.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbrqttker.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gfvojueou.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gqjnzyfhc.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gvfqvtlff.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/grqxhxkoz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gwuyvilsi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/grpzlisdn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/guuoftatw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/glydnaisn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gkvjdgaot.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gyszpuvrp.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gghwfaraa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gjuesqqzd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/ghlztgspl.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/grlebdyza.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gwliuqiio.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gbagxpxgn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gbofolscs.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gxxuzapfz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gmjbnprwt.sHtML


<!-- 参考信息 -->