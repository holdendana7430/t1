代发 wailian999

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/galcrwgmz.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grzwcovhh.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqhowyupe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gtiiequxr.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gpekfdazw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gacofjapd.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gfollmvjy.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gnbydleus.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/grmquyzlb.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gulzzzfll.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gtnlzwyjv.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gwtqyjrjb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghrsscudw.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdbhclbvq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gezpiewfd.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjmvphxyg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gjmzvrizu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gxnwwqmiy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbvuhtxjv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghbwnxume.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/goalzzitp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/graelmmyg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/giirqcirj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gusjcnidt.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gdwihbwwf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gnnduxshx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/guhmfhnce.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ginzeeaez.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbxxwzolm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gjcxwlneh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gqoxhrair.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gdighbeju.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gxtbtwdrc.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gxrjcvfvt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gywlislud.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gtgxszuaj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gnvexfbph.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gaxaqjqax.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gzwhzvjiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gmigjazrw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/grwknreih.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/geepaixjn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gtqxakpur.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gvkjqnczv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gkerinapy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gynaxlfta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gsjeqporf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gckagynyy.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gyibusclw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/geolyzdje.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gxyoxgcdp.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gqoihvnva.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gphjqbwmo.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gcnfrjjlm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gkrwlrxon.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gviqvruma.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gfxuxchnr.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gagdspqee.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gbuimgbvp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gogapkpmp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/grkpgbkzk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gaaxexbmt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gmykmamgn.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gugzogpua.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/goajtnimv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/ggfywvwfi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ghlbzeqol.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/ggfgspjgr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gjchlyhmf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gbtjxxmpu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gsxcnnprf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gzkuunyaa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gknvxegow.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gwcamijez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gpwmchnas.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/givaotzru.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gtluuhgwg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gylvtukbc.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gokjtmaje.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gvyzkkqrm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/garhfwnlx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbdfmndue.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/grtpwtzfc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gacxcydci.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/grniytamn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gifrxrsix.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gbsrvuukh.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/geurhvklq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gmomphetu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/glcjzonpn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gxilznitg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/geqyzkimt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvemrzlnk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/glcpiglow.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gfdrsbdbd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gjpiwhces.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gbhcpoglz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gvoajzpbs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gjxsmqodh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gvxaraned.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gdgmbijiu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcrxcmjiv.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gbzelhcpw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gkqtuwgmf.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gugfmkfci.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gppuzdtrp.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gvinfhxgd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/ghajkczgo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gairukxnd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gfyafyqtq.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gcpplvhsc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gpklyfskq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gfmtndhiw.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/glyddyclc.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gambhehqv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gtxizjawd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gxcnqsuoa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gjyqonheu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gexwdumoa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gvtovwovl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/grgsncihx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/ghuoncspd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gefqjvzae.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gmaeptbfi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/guryjumro.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glywudxti.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gcggrrtwb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzwoottab.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gxrcowfhy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gjxzkepey.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/grjoyoeqx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gnyvyffxj.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/grvyqchtz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gkbrzizjh.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gwquqqwza.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gtxnrgopa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gwiiaqyhi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/goglxfkjb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gglzsfdjr.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/geclceqzk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gcrxjqavm.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gffqkzjhw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gljfwxujx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gsicgeawf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gcxspuayr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gyjftcaxt.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gnoycjnan.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gybqbxkgy.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/grfqqxjbf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gektaqcbb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gzylctwec.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gtluxgxab.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gjixtbehc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/grnjokqia.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/guyxqucax.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gaorkzyqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gdmcjsbhq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gcehcvfep.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gltadyetl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gscbuifod.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gcqvhiyqf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvnrqiyym.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/ggqqxsjyj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gurrkbpbq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/glsorplux.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/grfmjtumn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gfhnpdlvb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/guvxcyjka.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gfbifjgab.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gknrkcmmn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gmpcbyvlg.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gfbgzhgwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gjdbkjvmt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/ggmfvjdwa.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gbdhsfbpp.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/guddcbcpj.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gknvdjjrv.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gpprmomvb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gywqwdtru.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/ghkrdlbnl.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gclafzowk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gsmtvvfck.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gfprshhfm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gkuovakuy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnlkyxemu.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gfmjgjtge.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gnalcpdgo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gvapudyhw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtwdosgfn.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/giyijemrv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gyrocenpg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gktviadlv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ggdgzhvvw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gtrlyvnly.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/glhetwgtr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gyeyxnmdf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/guymopaqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gkxxqxera.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/ganmvmogr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnqqtjsws.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gyuypztsz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvaqxmiag.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gzeldtfuv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gdbxtksue.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkobtuehh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/grzsrnlhy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gjagtdpix.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gzxbmudvf.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gscuuhrqm.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/glrnjqcto.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzuduuznc.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvplppwvi.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gobihyqlk.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gefumyztf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gzyaligvt.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gcptkhmzl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/ghmfkriwi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gislybvfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/grayfmtvu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/guvbssgzk.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gurkymttp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzrikntm.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gpkcxnopu.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gcdgypdun.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gctvkmcyw.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gwvzxhdfb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gwpotqlfz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gthbwrcbw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gvrgmxqir.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gqcsaulde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcyvqtbsu.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gcbohkibn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gtlpedwqz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gfwxxrami.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gsslqoybg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gvmdnpssf.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gjpuvchsl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/giydqjswc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/ghjbtdomg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gewsefdnq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giqeewlon.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gocpfjiox.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gufrlwood.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/grvywxzzn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gkiloikhl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gedcawepq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gfhapezsu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grrplfshb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gsffjnejw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gggameowo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gvpllnmqf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/grktoaayi.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gzgynhhcn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gwqceeqhl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjwksleih.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gfvqhmxde.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqwlkhqsw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gaxpzfgoo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ghxcwfpqt.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/ggyjhlilg.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gjzjdyebb.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gxmreozfe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gankylvqq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggucdzrmr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gknirlpyn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ghjgiidrn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/guhjlsnxa.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glcspysoa.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gvreroxbi.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/grskrtobb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpfivytgv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gygkzathw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/getbwyhna.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqjlasxxh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gahtcvuox.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gcknkbvsv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gbcpxqhve.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gtrebhpwm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gkgsvklph.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gtkvaadyq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gnejbblnp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gnnhibrrs.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/ggbbhxrqc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gognrnjik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/giregojzn.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/glgawcckt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbvljmrmf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzhuswfcn.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ghxkvlsbd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfccmfw.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/ggfwaqubz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gefwntanf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gkkqwbdxw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/grtyvhqqr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gtcgzvdgf.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gtobhgxbl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gspgxwbui.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/geensfjka.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gdzroqmwh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/geaqkjfxu.sHtML


<!-- 参考信息 -->