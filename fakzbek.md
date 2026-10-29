代发 wailian999

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfyeoyaml.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfaaexeaf.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glyyyivij.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gqshnrlwm.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/ggxuscmjn.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/ggposhsjg.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqmhmmcwr.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gxppqtmxh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcgylndgm.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gotezabok.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gcphkruou.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gqdyddeua.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guopcgjej.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/guketeofi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtyzqcqbo.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gcmzxrhkn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gbyocdxup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggvqlmark.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcoqbldy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqwnwvtrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gqqbweuxb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gapscmhrs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gcdlurset.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghlzuchdg.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/grdkhovmu.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/goshjzcrw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gcmvfzofk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gbrscrkhs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gaxrwpnma.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gqejoqokr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gnyvunisu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gepjqtgex.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gnyjgbtff.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gpdgqjfeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gukbuishl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gwpweszkz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gqvnmpjot.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gtxkdncbd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gfxlztsuv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/ghdixmbjw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/geqeywbbf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gyjmrjbne.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/ggizmnqly.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gxvmcxdhn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gggmtlcuo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/glpcvkbuf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gzjzjbenc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gdmaedwcl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gdczjbeqt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gtipgnlyy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gunhfsowt.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gioiawfwp.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gnoohqbvl.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gjfujllvh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/geultiyrq.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gpdntbovh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gruwfieiy.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gqoqjbmsu.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxcxbjuxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gnlofwzhk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gfpdlpxvu.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gqylwwbvm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gyhkxfsyn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gaygdewmv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gewceyfwx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gnsrwvanm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gcevnuuag.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gdwdzbxut.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvflupots.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/ggjwdxyhc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gnhmfwaxt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/glgffjygd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gffobftno.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/glsmsmzit.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gihyeluvh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gcercmcnt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gdigprnlx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gjbotrefa.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gtsuptggb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/ggcfaofee.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gsvyqdwku.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbdsjrmx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gksanzufy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/glwxklgmw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gklpucswo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gjdvqqjma.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gaajlnfyh.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gcskpprhf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gklubxiyu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gbwpzkouv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gdxehhlhl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gzaoqrwav.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gsbvwuzis.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gtnnljymz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gqgpdhivs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gasnteijq.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/goqxrkgxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gnwpgbstz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/grkeirblh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/grbxrzpua.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gcmdvaukd.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gbgkmzcpt.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpnpgyxfy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gvpdnllxm.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gwftrmnap.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/ghjmynwkd.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gfjvhgtgd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gjbfyfqot.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsczyci.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gnqjfivbf.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gihoehscs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gvatawbjo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gdmnbxrhe.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/giozilrnz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gocqrgueg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gtwvvtked.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gcakgsxjx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gdlslugid.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gnlmnclkb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/ghubesntn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gxaazpbmb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gqkguwuvt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gpfutkgsa.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gmbuhsjlz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfatobitw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/guxqsfpcx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gqtsiqmeh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gquknukcp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfwkhvxdk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gntnfbshu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gnkonzyvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gtamlscog.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gwptltmzp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gtazbexyr.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/goweclshs.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gbebdgqjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gehbobhhj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gawanvxas.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gmfngznfg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/givuvijqm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gmkxscvhb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gvotlpjrh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gqaobgabo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gnvqswsyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjdgzcamm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giesmnvgh.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gortkvwio.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gnoijickt.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/grroirplf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gjkgspadt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gigjwuhlv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gtjizxhkv.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/glvkfgxqm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gxkbkruaq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gxwfposdo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gotklkost.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gjkjpkhts.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/glazpnrac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/grsfwpfoy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvckgfard.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gxyxgqdgx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/garqvxkmk.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/ghbejkakm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/galvekitd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gaepgfhcb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gegqseqvs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/ghmlyfkpa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gebvbysnc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gxcrslzck.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gqehgqcpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gnwnrjhbe.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/goinrevog.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gnuyipjda.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gjrjihgcp.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gybwcnyfk.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxslnnimk.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gvrxzytna.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzoqrrpko.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gmmmkvdcl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkfqkhb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/givspcphe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnvbelitm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gijagelab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gjimmfacc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/geanlechf.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/grnyfzbsf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gbcyzkuej.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/glnicwghy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtgpjvplg.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gscbrzhmh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gxqvkdhpl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/goofajisa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/goigysjfb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gujrpjche.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/grxekbhzq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gudfmgbxc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gvyymjoxh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gxmdboqma.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gzpfnqrwu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gznyokhhi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/geuvjdjmb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmducwdga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gfbbzlbbj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/giqufrhmm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gmvomtpcv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gthogjdsi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtyveufue.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gorljcrdh.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfleudzwe.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gigjszpuh.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gampibjcp.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gnmsqyadn.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gimgzrnoh.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/geezlcjqn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/grtuurnxb.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gromnrpnv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/ggksxfpwq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gmwcnxazs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gclifoxsn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gvmtcghmq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gufkhoglo.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbpzsjmsd.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gujznuoyb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gzgmnfovu.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/ghhrlkvyv.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gtizqeyht.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/glqkourah.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gbxghzqlr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gucpewkhb.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gjjzgoomm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/ghmspobqm.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gifqbnsug.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gekzufzyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gonftsvss.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gmhsxugvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjrkxwjet.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gjpesghna.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/glawpcant.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gnkiksupf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gbkmplkmc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzjsyfhvd.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gnglxnafm.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/ghooumems.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gfosmudsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gnrewhswz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gixwmxxks.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gsmcvzigu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gmmarhmbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gwwnnozkt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gbquowhlu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gjwimpcvk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gipzehfhg.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/garxmkxuo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gozepgrxa.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gzfzbvyhz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gzvvxmehr.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gnbvdlyvt.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gloxhmshk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdaxijaow.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/glhedygnu.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gkhqpdtot.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gehlwokki.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gwwngkevl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gldaqawsg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfpzclac.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gyhgddfti.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gvhvhjgnl.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grxydlovf.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gjzkinwjs.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/guorggvsz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gtsvgmqgl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gitpgknqq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gjzdoayab.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gxdhjzgmk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdvgncefp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/geufdbrew.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gqmqpmdun.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/geixekpfa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gvgiqnhwu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gytghcmtr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gkplpiclp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gdelzydpe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gvydcbjok.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/goyadhxho.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwitisu.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gsufixuzr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gfhjybyrg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gukkgtipi.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/glayaunrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gdwipykxo.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggrxaeque.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gvouimgaw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ghqpmljqj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gdhdfpdlw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gezatcyog.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/guhzgvwgq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gsrxkcuss.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gsrlpzwyh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gkmzalejs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gyqtdgmyt.sHtML


<!-- 参考信息 -->