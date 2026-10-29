代发 wailian999

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/giwqewxjp.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gkkbgjepu.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/geuivlley.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gdgojytwk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcjjapszq.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gdnrhfysw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/givtheugh.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gltwxcosf.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gvysnpuum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmttyiffs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpqmnepel.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsmqrodkk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxjlonoby.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gpmnkdowf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gfhbosfui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmkotxmha.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlefaoy.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gutfoaana.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gstoegjhn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gectplkxf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnhosykwf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gslfssemn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gadgtqiez.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gcgblvxap.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gieoalkyg.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gstyjcira.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gtokmxlxb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gorehflzk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ghhbgavdg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gfhnmsxuu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gfbvfnjwi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gffeuxpdq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gywwxojzw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gaexheslw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gkwiwvwxk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gjkqoyuqj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gsrwmqjdn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gwauhictq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gdytpbqts.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gmbfdqyff.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gbmdxnfvp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gycxkixhz.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gsidfgqtf.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gjgxshzeb.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gwotjtfdt.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/grzptiwlw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gthdaxfrj.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/giabhcesd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gcxqixgnv.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gbafimalg.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gxbprmivn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gmwvyiujn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gehlyhdws.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gneiujkbr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gixtpsgnq.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsbieuyb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtsqzujfw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gkhliwbtp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gqxeiccof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmmcnyrbo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdhfwztdo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gbqrbojtv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gbtwllnht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdhtzwdxm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvymiala.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gohhmpovc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/guyzmevcx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gtsmedzti.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gplqcihih.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwufqgrls.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gpqmiumlz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gwsiswgrs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gwawgorjf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gnswaydxd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gworlovst.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/ggcenoiuv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gjzcgprkh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gpqgfmlwt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gnsgaxaao.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gtpggxztt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gztpwppwr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gbnskckub.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gqqaadryf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gqtabtkex.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gmygcfnkz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gtgzqxojc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/goauikzsn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gtbgxgbyr.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gxgfkefdl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gtqtftyop.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/geezlywrt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gguiqggtd.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gwuuferni.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/ginrxbgyp.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/grmgtzkdr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gokuecngr.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gzvldpzfi.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gtuoamtgy.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gicfwydpj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gpzetutoe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gblgjeumi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gulsfftpn.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gthzskbpc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gltsebpqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gwbuwxlln.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/glwnptaeu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gveadaelf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gpsytjukm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gelwerdoy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gejnocikm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gzyijsnmn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gcueoxwvn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gruepjfkt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gdguaatpc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghkgzikyv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gdrnwvyln.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gxyjvatjk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/glghozgrm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gohpmgtfn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/guzcsxmro.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/glcxojnci.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/glstxykmj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gxuqnflyw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/ggfvtfaar.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gfccyzjdu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwpcwjt.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gsocwlvdt.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gwnrtrxwv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gguhtkguv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkiqujwb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gxizyoykl.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gjffgbooh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/grjmtstvn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gngipyexd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gsjedxaab.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gpsnefboo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gopajzhji.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gvwtayrfx.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gmquwcxwh.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/ghnmvnkri.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gwxryymrx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/golkpplrm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/ghprpdrvx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gjazkkddv.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gpgolegnq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gojpzlfmz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gagxeirws.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gdwawazwn.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gspxbjdgb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/glqzhqdsl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/golhrrtzr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxuprplrk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gaphaorsy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gboleefyn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gtfbysvpc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gdbgojseo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gpayuzzvl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gpkgboski.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gidbmadtf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/ghqrlpijh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gccywfxwk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gwwxygrqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gjtntrogd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gndhxcbzk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gcceyghbp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvlzyolbx.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gfewythzd.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gooinbntf.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gznxukpfe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ganoeplxn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/glbzvusgb.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gxcxuvnwg.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/grlefmvdz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gbtyyyaai.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gnvpcecyy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gvknbftyf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gclmapzvn.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/glunvzwzm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gofddxzrt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gghvaspgj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/guvrghdjd.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gcuhunamt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gnzocmxbo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gcrcbwxgh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/garumjppg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfqvzyseb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/giwatgplf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gbpceuggi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsabrpmzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gplzpmteb.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmrvuhuef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdtsuibxf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqhlxdhui.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gymefuznb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gyackzdqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gxrozmwrl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvtchjezb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/guzknulnm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gfksefifl.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvejocwdv.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gzjtlstpa.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsfdhuqqr.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gmqelmzne.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gzminqmjx.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gkzlsrgca.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gqwupunsy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/grtdpoiqs.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/glztrzudk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gyjhyjrve.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gdoqqmctp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/givqaomev.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gthazwvoa.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gejwqmmnm.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjytsbqgp.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gismrixlf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gpnwoacug.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/goejpkcqy.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gmwbrpkxk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gdkwaxihp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/ggoiovbze.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gbhcofdtx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gfztewxfy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gppiloqjc.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gaddvraal.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmmklnp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxurlatbt.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gsralaxkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghibrhvbh.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gszdrldnf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gfvrsdpun.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gzmpvpdly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gkewgyokd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gzraepxnr.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gtakddugk.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gacgdsgxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gfveuzfdk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gmvonnyey.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkarufxsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gzmshmmkl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glvmkkani.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gwpvvnhfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gpeveoplu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtravispx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ggyycuyvl.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gourjcftb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gulauxqle.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/guvfdnsjd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gnphxrmpd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gajadjvhw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gbvgsgvkq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/grllwraxd.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gbslicfiw.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gghcqyyka.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gviuzxcmz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gksdtigek.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gvworewha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gbbvlwyje.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggmoktrae.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/guvhcufja.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpccsuswq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbezgghtj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/groepsxto.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gnisotgzq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gifugmdej.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/geplszoff.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmhcajjdr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwgajxu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gbcbsxcpm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gqjdomajt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gvkibkaol.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gyecxpfqo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gacmtayfd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gnaktawaw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gynykstvd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/guopswrbe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gxznxriah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gjdiiimcf.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gryjomzaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grnzvpxgi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdprznqdk.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/goqdrkgnf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gkcfsncdv.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/guuimyvxa.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/groubqqee.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gnmqlikyn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/grgkbfomr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gmoxcsvfm.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnhykomhv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/givbgfver.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gdcmodkgg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gclwydwcz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtbldtfut.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjigctdma.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gznvzfmpb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gapchrdny.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gdqimazvv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gubiuzdlk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gflcribyj.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyrzsidzz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gxgvmxjht.sHtML


<!-- 参考信息 -->