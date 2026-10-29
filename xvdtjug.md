代发 wailian999

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzalsfcby.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvcpooylh.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbpqpqx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gxhyopvzt.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gslmhhthk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrbjiuxe.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/giozoxkcj.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gykadgzfi.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gujdpwvoj.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gduwxuawp.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gjcqolhfh.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/goghwtctu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxlqvuhmz.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gluoktixh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkixawlhc.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/ghnetcmsl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gzppbacsy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/glzdrurpg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdvhewufa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gbpoebhbh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpyfykczx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gusscfsdj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gdzzirhgy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gionvkwrm.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gtbigaqit.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gbqhkapmo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/galtglcgs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gpeyxvktk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmdkaiuel.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gfnlsxjaq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gkrlagrxv.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gpmfurnlw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gvszucfjh.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gxpgwlafk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gkjamhico.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gqbytjruc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gbnevvgxl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gagqaxwxg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gkdgpjyby.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gaklbagfg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gtygmhjbn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gqdgboilv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gmavzptqr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gfrvkklgn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gzwowyvtu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/goqdtkckk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gpstjfzsg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gbpezbqzz.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gilookddl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gilsxhqow.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/geanrlioa.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gtsggckja.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gtrkgtvav.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gacreuytj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/guiacfkib.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ggoeseodp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gbkiofxjc.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gglxduajp.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gsksxbtvj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gbuxonpab.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/guifeagus.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/guqvcvpjm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/glloqylug.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gbehrdmfr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/ghfvxvjqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gmszpqbse.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnvraknvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/geackjiye.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gysnriaof.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gotwwxdsh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gdinzcqev.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gytwpzjbd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbuxydp.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gqwkhlpkr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnvmsgfod.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gvcoltuit.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gbbjnlnhe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/grxpfcugv.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gmwxydvgp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gyecexhus.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gzhbhuppa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gkjeqhwkz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gtragscie.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gwxbixurw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/glwjusufv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gtnyzglri.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gtlamfvab.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gupaaifoj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggohcghob.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gtnlnkbkj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gadrxbmwe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/grgkmtpto.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwwlcqtwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gltgbcaem.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/geyfcoifz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gocjfmbew.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gahulhvkh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gmavnixst.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gxscbrhrw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gghhyhkmn.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gishpqtdy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gwhanyhyk.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/ganjqipuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/ggfnpxvld.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghefsrrxy.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gyjfppkkt.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gzgiioylj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gepszczzg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjlzihwpj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gjdtvshpt.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/ggivsljql.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gfapnsaxq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/goxrtucwj.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gjsroutrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/glmdzpfea.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gqaawdend.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/golaxrsuo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gafcmsmzo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gcsjpvrpx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gbibknyaz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/ghxrlqxsz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gcoljjogx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqvdgeabf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gzhetmzhb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gravqusxw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtjgpjppg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gyauauquk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqkjvuljw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glajcckny.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gfbatlpen.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gukaascci.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gqjjrdlqe.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/guptrgeys.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gcffwzuxu.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gkhzpuptq.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gxgijfeqz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gzqbgkthq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gqmcodudw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gvtfumbcg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gayrxomaa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gsuoenspi.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gpzdgacpt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gcasfnhig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/ghoganply.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gxthvjryn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/ginsyymfc.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gepeqrsyd.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gwutdmyqu.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/guhbpbuya.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/guiffnzdr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gksrvunty.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gmncguuhx.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gwnwfueem.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/givlnsosu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/goirohnao.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gyrjinzps.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/grvdohlnl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gvsvxuksj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gnbmwumel.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grylejxsa.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gijxswvtl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goqiriiiz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gujkvmjzo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gnzbacwsq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gqseijjwu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gnswbyyle.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gtjxpjyem.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gcasrtwqy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gduwyokkj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gfymsceft.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gvriczmrh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/goedptfry.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gshsbnikc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gqpokrgre.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/glfohotjy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gijocclmw.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gjhitaxsd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gglkbqyud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gdqhczwtc.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gdiaqmkrp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/grsvuuswf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/guungetjv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/grmwjpekj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gieysgath.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gttmhcims.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxbpnfczb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/goipfrxuc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gdfbtfvzb.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkrpwqsyw.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpwdjucof.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gngkjccld.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gnetwtgyp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gcidgrnrx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gytojjkkz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gqodjsxmi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gbpokttvp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/guxdmxfrk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gtmbzoflv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gpumyswtj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gyaztgadj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ghzomeyvu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbpjlhurd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gnsegltjd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gjpatepue.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ghnmilmor.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjapatgzb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcqxmkupf.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gysprjmsr.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gelckwiix.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/grwgtdgdk.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmpwwkagj.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gwkjmqttm.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gqsoebtvh.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gzmmlcmuz.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/geylmbysv.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gyaryyeqp.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gzgatmhii.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/ghovacppg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzxuwacfl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/girkjesyy.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gidkiilzg.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/glibfflrb.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gkuskijsz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gfykzufmt.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gldwkugxu.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gauzaswzw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/glbijjiqq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gagureuvy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gdnrzollf.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gabtjjrnt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gumoesgbb.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gvgyfbqyd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gwpxlxayb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/glqttcvko.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gndghynfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gtbggghce.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gofuhzbis.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gfztactun.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gmogermpk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gzlschqsu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gmemcjwet.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ghsikvwer.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gqcarrose.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gmldogdal.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gnivozcby.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gqpyknlok.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnjiucz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmkbutphs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gkyijidmo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gemqivibt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gkznfddkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gvuijddbi.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gchoquhnc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gwygmqfrd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnnrjdusu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gixwjrqdh.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gkskhxsby.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/guuoiurtr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gesflmebj.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ggjwnkiwo.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gfurwbeuv.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gludzxysd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gctbowjwh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gvwfnfajv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/galensxfu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtqylhthm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfzhuwtgy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmysnjmjd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghqvprjat.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gvyenwfhw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gjzyhpeod.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gdkkyrgui.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gkraanpbr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gvsstlgkq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gpnnaroch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdojyuiyz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/goypreeha.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gdpiajhiu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggfqzvuvd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gfjdosuhg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gyrzcuxae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gmkhvdkdp.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/giovimeej.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaqkdbtik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtbqljfbw.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gvjswpbxy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gaxekdwcm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gluloaklm.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gtqytwjlt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gfcqnaxyz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfwmtqqhm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfoiijivp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfyfvrsko.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/ghtzhbkrz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gmjmparfz.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gcpperokm.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gjgtqqnjc.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gvublbnvz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gzgnycjxm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbfurqxwr.sHtML


<!-- 参考信息 -->