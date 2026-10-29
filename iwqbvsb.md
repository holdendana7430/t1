代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/goxkxiivj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/ggfxwqvva.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gutynvzri.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gjtfxvhzu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gwhvczzvy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/guxcrajgn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gdfocnsou.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmqchkpj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gevsxioza.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gykzkisfz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/ggaykexwn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/galixvskc.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gzmdxtnwd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gpbxcybip.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/ggrsvhkpx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gigxfwzjg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gguyupmdp.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/ghjofoicy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gciahsqsq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gmumojxhk.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gztkpfmhz.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/guccamvvw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gsuqllnsr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gcyowzepd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gkedlapev.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gpylyuhjy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gwsifpgjy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/ggsrfriod.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gldieejlp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghcbtsmud.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gbyrjwpmk.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gulrkcwhg.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gbaipgebb.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gngwbtbdv.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gznkmamni.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gpvybfgrc.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gapcptyke.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gourygueh.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdnmkgfiz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/ghilbnytm.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgnamqt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gxvetxdzl.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gcejgxvmd.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/greuvffwf.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gjslwwxko.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/grwlonpsj.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gtsglnsdu.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzqymiabh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geowoaonl.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwjrcsdel.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gogidjrhp.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gezzqnbhs.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gnkqxoxcb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gehamqkee.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gfsfwxzjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gslzqpckd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbelsvaws.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gktcbldbu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gztouxxku.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gkqehxiaz.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gwthsopcj.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gbtusqtaw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvnhmdw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnrmlvock.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gajiadszp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/grcbtvjil.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/ggjrwugyt.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/glepgjecs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjsbzug.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/grqwwasiy.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gsaccrllm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/geynbrgis.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gdfbvsjlm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gjmnwilyg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gwtwafaqx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gzbrkxhlp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gyjjabuje.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gdzjznciy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gofzygmmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gbrzylpbh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkquqnhzo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gyxixemzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gwyzdvncz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gzpgfhcoh.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gbxnasxhq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gzkdkdjmr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/goofcytnv.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gvspnzqrm.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/glcadxgrt.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gwpfxswkg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gguwlwjug.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/geymdgxsz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/grvhkkjtz.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gahhybzee.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gwnjhayku.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gtbutkjyr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gtjnwdhlj.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gawjkanuf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gfymjqtnz.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gjunljxmi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/glagrssgg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gclksdxqq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gsragcyen.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/grqquvims.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gdouombbx.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gqulqyjgl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gjtlqbnxa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzovkbztz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gjbciisrn.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gushuofpr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gbnqyfbgz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/graujtduy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/ghbjkllxy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/ggeqtejrq.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gjeymqtyc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ggevslnrx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gyktjdvix.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gmktpbehs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gnhmlexpw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gnqhqwjas.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/ggpyjhgxa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gpzmecezp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gunmrofrs.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gxvihgrjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grgpkemhu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/grmauwjzg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnrhekxjb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gthptxebw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gbmtnyypu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gsmglfglw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/ghwtonjqn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gmjdtubih.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gmebtnjyo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gzzndlmgt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gyvztuqni.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gfqvsbopi.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gulysfqjn.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gptqtqklm.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gnkonhuko.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gijcgklnu.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/grwatngbo.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/grvgqvuxk.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gpowcmoec.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gcgbsketr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gwdebknfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gcbnutnhh.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/grjeqqewl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gwyvdzldj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gvkbogjkx.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gnxqthduj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gkjbmtgst.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gitwyvhru.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gsepzbvpq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/ghgdgvqxr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/glirojgrf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gxjazxxxc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gythzsimh.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gaqbbmlsl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/guspwdmec.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gnsxmskrv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gtppjdxfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gaooyvrbg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gwyipsrhi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcvancxia.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwgnhmsvf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gpdoucqze.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gqiqxjtkz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gnaikjumj.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gsvwualoy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gmlauqbsc.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gngfwbcev.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gmrjjipzk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/guqattdbv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gfxppylih.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gymjbbszs.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtbkqxygn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gdcjxbmsl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gojqdvqgz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gngabvqoh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gsoppcbui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/grqsoqcct.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/grtlfmfcv.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmnbiegxz.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gnfkofnvd.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gisrwxkoc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gaftwipgr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gmmspvgjl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gxyncliyr.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gyxkuzito.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gyobmfvpz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gjjgjsiit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gmvzhddfb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqqqefowr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gdwsvykne.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gknvabvef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnqxpxqhi.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/ghbdpywqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdjixquiz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gosnrrpnb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gunfdnpdf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gnwkpwfld.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/giaswmpxt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/glgkiwjbj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gfjznnade.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/ghcyraodw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gadovovmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gechynjyu.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gupxuhosl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/goieassct.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gjymzvvbh.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gbfzwnjcs.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gnohcigna.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gzxvntflt.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/glbfcrxhk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gzqagxrrc.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gptpyiceq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gjjplzcvn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gksidsevx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gswrageso.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gonbqaxoy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gbcitllxp.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/guaxygcvn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/geyrocerz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gqwsgleed.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gwwfxmxaj.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gioxvsxxy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gnevqmxnf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gezrufjrx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gtdziwzqp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjlkihsty.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gmnqzhlvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/guxkurkzb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gdkfxsyif.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gctuljflr.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gesaukecz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcotzfysq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gunqhncnj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxpikiwhg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gygiupmyz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gmqpyhqdq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gacgguvri.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gfmjjcegi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/guytuayzc.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/grbqiwjdk.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gxgrvoicz.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gdagrumvh.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvglbuxve.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/goccmjvuy.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/glcfozrqw.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gemwlbwwf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/guuwscbxc.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gauuedqbb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gfnyabmsi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gfjvtrtrr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gfffyehya.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvxmgelyc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gnomdgdeq.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gcwsbnejv.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gzkfamfge.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gavvtswqm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdwrnrobg.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gklrrmknm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gnzilixnx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ghljpjloe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gobqbnkeu.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gqzetajmo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gkwcnwzwn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gxbpoweta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gseoctjld.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gmmktvegw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvoasgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gcavlgokt.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gfobxkdxo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gantjyfms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gsnrhlfzh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/glwroclsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggpktydtp.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gehfmguuh.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/giihawtbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gpaobrgnp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gpiajqsrx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gyxlbczfe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gjbxpvzgv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gtgyizlxj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gzcqdiuhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gpvxdjnkf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gkpjmmste.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gybysivml.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gnvprlkpb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gdgdqefgz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gaowflvql.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gqwxfrmid.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gisoipqlp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/glqmnntzn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyeokdufz.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/ggdznzhix.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gcnydgdxp.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwbnyamjh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gndvhetpn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gobbgkjuw.sHtML


<!-- 参考信息 -->