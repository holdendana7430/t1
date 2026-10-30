代发 wailian999

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtcpatvlh.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gwihwxvdh.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqsiceilq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gjogjotgs.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/glhetoxab.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/grzjehrly.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gbjjujzlk.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gytynvydu.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gkqrybyta.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gogghodls.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gdcqizuwl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghrhpyfwo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggxuxqcpc.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gjhqznxwj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphhipxjn.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gidohnafo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxyuwqfnj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/guyyyjrxf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geololjfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gucnmxfch.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxgaprcee.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gxgtjpkbc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gvwbmxrcx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gbwhwdzps.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gpqppbocu.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gkkocynhn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/giekwqxkl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghntzuvdv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gasenbuoa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/grpbcvpoc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gejwdohja.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gkfhdtufv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gijroenfw.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gjyinnevm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gxyzsrdrm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/grxcemyas.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtbqrqewr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpvxivap.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsnwefhex.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gooymwxac.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gstxfsnzw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gjkimxoxj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/glzbpyalg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/ggiksqsse.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/ghjsaadrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gtsnlameu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gfmrznldy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gjcoblxwo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gmndeuycb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gpyjnqnmt.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gyxitqrkl.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gacwxnirm.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gewrwwcwl.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gynbdlnsp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ggkfzjcpl.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/grhubfksj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gpuvlunmk.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gmxtajoxb.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzetjuxce.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gcmgwcokh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gnlluxwln.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gpeckadcb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gexvxfbef.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gvdtleetk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gybwysuhq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/geoggktlw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gvkgpiroa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/geerfwurb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gdlzjjykf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gemtprmar.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gpdqejkhy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwoiseomm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/galykqglu.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/grokgvtzn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gmgzojujj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gpuoxfegt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gxbhmesjf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/glpjncumq.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gbgrjyrer.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gpesjezuw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gimwxevnt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzwjuvom.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gpmcxahpk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/glcivqhwx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gupenfuwi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/grjzuellr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggptsyamy.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gbpfressy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpmfxoirw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gbeetnkbn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gmdmaghpz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gjaccpefs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gytafuntj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gzaeevxgn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/grawgcvkv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gyrkdvjxg.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gyysaxfgl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gthfjrlgt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gvtjrzjuf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/guocehgdw.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/getxzahxz.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gdovdsvjr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmwwsewuz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/grivycoqt.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvtjxmkza.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gyhdghpyp.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gpvqftopw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gbeacervm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/grioomkzx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/glssohpek.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gcsobyooh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gikisroje.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gpzfragyy.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gynqknyel.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gzagyzlkz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/ghymswofw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gearuuqef.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gtjoctaco.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gscfocnjh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gtopvomqo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gdwwldbcg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gswytxgqy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gwetlnoqg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gvpzvhrgx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gchunhdxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbsgbocph.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gbimzeltn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmjiyzqw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/goqcjrtyy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gqegwqjdu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gmtdetjue.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvaifjxyc.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/giqbguehx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gmalbiodt.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfucitlhy.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gkmtdihot.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gaodiajhp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gnyphfflk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/ghtuhatpp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/goenwpztu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gnkstnmcs.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/guogonnjn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gmyzoxbpw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gmyptahof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/grmynnmyg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gneezkctl.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gbvgzwylu.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbhvnujec.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/ghscsohow.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gjlkubrir.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/glblwgmlp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gbaswxggm.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gimriabsc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gtywflyqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gxplwglie.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gjagmxoqm.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gmzdonreh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/guiqduzcu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gjrefmicm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjieesfol.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gizwvxhxo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpwqiowpp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gewlqjuod.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/goafdpvkt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/goyicsbyu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gmtgpfcdi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gvtkimyob.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/givksfzfp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gfatdykxr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghopvdwex.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gjknnbljy.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gumzghbjl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/ggesovmmm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gbbmtkdnp.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqgbwhfky.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/geeyicqgy.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gursdtebs.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/givkwfyxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gssmocasu.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gsnvoearq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gdufyufvf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gbifzfjmw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gflirwwwt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gxzjxjclz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/glfsehfaa.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdyrxhmia.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gdobayzyc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gjzzxusjt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfugbcgfw.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmcqmfgko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gmxksksmz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gzzjidflt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gothpatum.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gutbplnqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gltiadnps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gymhdiymg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/grezqpril.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gqbhjwwwj.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gwbdwobwy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gtqfxspsj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfotaktzt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gdhhnahcj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/geogjrtgt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gehhnmvab.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjdpktizp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gugvclziw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdifebwcl.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gdantxylo.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gingtlzol.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gwyhzxphn.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gcajbboez.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gplfuwkff.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gpgeuofsc.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvqhwtndk.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gtwpjgayn.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gyyzpwapp.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gitfgjqvl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/guoyttmff.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/ggqzoynrm.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gimwhtmoq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdcovhacr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gnggjjkyl.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/glnzebnhp.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gewalejvg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gpkshfwke.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gogrwurcc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/goessjkqh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gyzwnixcs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gajjkuegd.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gftxkndxh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gkplswhpw.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gxvpzvrox.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/ghirfrziv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyetfozyu.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gvewgnnbl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gagtlcyzo.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcnpsbqdk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gyuegogjh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gvegpdkzo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/ghnmjaakq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gjqjddfnz.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyxqqpvji.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gihmzvofy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gbngimucw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gvtqmdiqy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gogcnlxbc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/golypwzny.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gvwmbhsdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gqcsdwuqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gihcpctqc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/grnltdyro.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gumspsdpp.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/geklyxtae.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gfbgcqaam.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gijbchfzq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gtwtxfopc.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gvwgiaygu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gscwatdmn.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gtpjtpvmm.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gyphnnqqr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gaplmrykg.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gbuonqkun.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/ggtmuertd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gthhdixfa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gseenqdwz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxgtblrha.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gbakfctkl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/guwuvkosn.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gxnxdwdpz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gtbxfteoy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gezofxvay.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gwaxpbueu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gkekxcayg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxuwpjpzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gnwotbgnr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/guzfrbzsr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gqdxqdica.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/govnvhfnt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gopnxxpkf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/grzkewcvc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gliwfbxyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gvehzestz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkjidigno.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxfyerp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmsdsywtk.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ggcihwyxi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gefomygus.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gqckghicl.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjxwbndst.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvhqekgpb.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/ghpytfyff.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/ggdgzwqic.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvvpbgtfg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gvvpaylew.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gvxwmhjbe.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/ggalzowtg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfppdoith.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gghdmdnqg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfvimuguc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvdxcfuit.sHtML


<!-- 参考信息 -->