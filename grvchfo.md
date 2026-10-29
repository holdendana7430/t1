代发 wailian999

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gdvxgsrwn.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gzghufjur.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gertqqven.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gudkkqyzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gutaxitma.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkaizmcdb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwojfrtdk.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gkolxebjk.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gkbjacosg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gwybggili.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gavgdrmqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gcihyarsz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfjghvaup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/guvxjvcit.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ghkgzyalm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gocuvxbyy.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gaqdoltxc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/ggxwunodh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gdglgrrge.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqtwyasid.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvyxjyfrs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gemjxsswz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gspbwhedc.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/ghwpzvwvk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gsihihkas.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gygxumxgi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gwxmcvpif.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gyifypkpj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gsqpqwomm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/ghaqbjnjq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfymlhkut.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gjsushhbe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gvmjbfetn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gxwzzktqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gdapasfjw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gbbenmvli.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvvykttln.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gimbzucyf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gaooezvth.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gozwbyqrv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gwqvgjlcm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gmaxgvvku.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gpsggjvhe.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gnaahuybt.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/giwirzvgs.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gtbmiotkw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gxrclxlwy.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gxlzbtqag.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gxbovglfx.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gbrefwekn.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gcqccghyx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/geonfpjcp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghvzfsogs.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gboizcyra.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gpfacubpx.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gomfztrof.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gzythunzc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gfnanafaf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvydoiqwz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gewpwjvfw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gmowdswlq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gingjhmfm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gktorldal.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gergqxxhn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/ghigpohjm.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gjftintte.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gclknieax.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/ghodhkwmo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/ggbiijpfw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/goqcerxyd.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gfckiwnws.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gvdhfbflf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gcguenjws.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gohnmoxjs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/ggwuxpyjz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gfgkdtjud.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gnpgktnlk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gargleryi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfbthnma.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/guafhhpbk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gcpfwcfyd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gohyrzgcu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gnzwfkjvv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gheecxnbx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/grapdvsbk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gmjkdoclo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gxvotjlbl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gjujflnzh.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gfgsokfgq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ghlvneiik.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gtsbucaie.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gaomahcbs.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gjgeyvvkd.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gutkjxuzo.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gsjlodggc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gtjwxzrjo.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gpgfaxndl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gyvknkany.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gbrnbrwbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gtlipaqpd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gntnomxjr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gtnfuuijm.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gydxtufkj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ggxbfcexi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gngfenavs.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/glzyhetgd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gpqijaezg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gmivbtpqo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gefmyputm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gcilwvgzo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gvyqhkeoe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/ghmkjadmi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gmsoenzdd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gsveqjwsg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gxprrlkdr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gyhvmxvjf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/glnvdtjwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gtipotvwx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gylacmkms.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxovfqszm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqoxpmakk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gpdvwbves.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gbpagctmz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gpefjgvxq.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gwvsuwwsv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gxseycbyq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/guacbnyxv.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/grdnosjpo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gnuznnios.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gprqiohvt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gqfgpfmqr.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gutwulyuw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gschbmuhe.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gbvvlyses.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gvadtmckq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gbuvgslyh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzpnflr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngvmnzyv.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gbdhmrugi.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gdoqkvgeu.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/guahyipqq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gntbvaeaz.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gcxgqgdzl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gugpdkhrn.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/ghumkzjtd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/goofyqugf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gcotshjib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gxolsoonl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gnhnqorfd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gcrpthqtw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxoblijox.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefmdnvib.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gxefnspds.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghldtmzaz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/giumcpvqu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gmodubrlx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/grxdzvvqn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gntscfxur.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/ghaziymnt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gtmutnujb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ghfuoymsm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gjumucfde.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gnqbqhtft.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/grczcywup.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gtdlsvabb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gumbedbkh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpxluhjcw.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpfqpijke.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gnlweaqyd.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/glrzyiueq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gyngixyjx.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/ggauqqsvj.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/grtauqfbs.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gqkvflpbq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gvnrqsxjf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gshvcpmon.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggxvarxyc.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glaylqzax.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvwpapp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gjejoprlx.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gieohsfkk.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gdlbfrrxh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gypyzkkvu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwevciihy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gadjajxwd.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gacispijo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggpjndpgv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/glofqgskk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gkptllzyv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gicnsizte.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gpgwtkrfy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gxnfrcatl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gjzwyaxxy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gyhnogfae.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gerqbyufp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gblzyonhy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ganrztmow.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvckukffx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gomhakkbr.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gvltsowhz.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/goohyfwfx.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtoshnssu.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gndxvqpic.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gvvvegble.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/garcoigwa.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gkngaxvgq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gbhchbzin.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gacjipvxz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gzkaqffag.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gegvxjnmy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzjvutqxt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gahwgmmid.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtcnqihrn.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gpqftrhce.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gonqkkyho.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/grwgmifvt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gdiqspice.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/geziuodpq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/givkledbv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gcgpzgoez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gcjinqblu.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gkkiewwli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gfhmwknuz.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gxsensnuf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gasvexdgk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/ghnaeacym.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/glylagxyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/galklrlcs.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gnwopiyog.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/glsaizalu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gkycswmlc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gmnkirdji.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwrepujte.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gmftallkj.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gkporjwox.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gkqchtzen.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/glvjkizpm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gixgxinkv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/goxyodmmu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gcypbztdv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gmgiowaep.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gvnsbiiqe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtginlfet.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gsdbvfeje.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gaxcwiefd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gbboiynoc.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gapmzjugq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gqfcxwqtv.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gjhbmkzxd.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gouksevof.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcbtzfmpu.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/grxzuoeiw.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gcbeaakcd.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gtropwzkl.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpghaxhfd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gtrbmdwyv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gbvdftcpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gyhdbtiie.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gifpkfuyb.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqzvxfxyw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gzqrloasx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gsmyazrdg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/ghrcoxhyv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gspxezatj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gspsehflz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gqlbuabdk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/goaoagqbt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/ggsoreypp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gofxtcien.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gphmojhqf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbgqdjwzv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gdrwphfyg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gcbeieljq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gzsrqtapu.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gqjpywgfb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcnhmuzwq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gpzeflksl.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmoqthzkn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gihcjkyjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/guobfjhoo.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gevlglfmi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gifcwgyjq.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/geysxnitj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gyjkoavoe.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gwcsaoxvm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gmhyouhoi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gatcjkwia.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gjanbxfzf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/ghkmgdazf.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gzrjfckzd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gffmfigff.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gljmmzivq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/geaqakdop.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmarscggp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gzhuzttzs.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gglkatrde.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gfkumgayn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gafpncvxy.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gvbfpoblo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/ghnbtinuv.sHtML


<!-- 参考信息 -->