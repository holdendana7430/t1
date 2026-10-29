代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gjqyycohf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/greznqqnq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gqdkdsgcb.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gqkczbxcc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/ghbjtsywd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gzspmrzmx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gucriquza.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gzbrgjffj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gxwakggqh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gboanenxq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gwsyrgodk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/ggooioeoy.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gtgbpqeqa.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gdygnvokg.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gtxjaljbe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gxcwcckdk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjforqvgr.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/ghniypsau.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gvqqpcozp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gkdqlewrz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gkincdjyt.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gelsmvooa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gnwfnlnsy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gygnuljvt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gavhgdbth.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gnwhcraox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjgljsefq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gmndlndfx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfngapbst.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnrblqztr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gcgcwqqwy.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gslkqnbhe.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gyqilkshc.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlqgwbt.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/giczcymwl.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghfbnfauk.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gfkbhvgyv.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjlyqfmaa.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxwuixldh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gxpfatqkp.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gpkzllkjs.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gjwgilhkz.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gghtjiotq.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gnhmdzkwu.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gghqkhalq.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gjnturbfv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gqpmqlxoe.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggtvuinux.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcipqlzcs.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gaptqdkrs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gepttztzd.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqfzdjzwd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/guvuivsvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grabgdxpp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdzzrwnxx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzhbcvfoz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geakofawu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/ghpheblrr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/ghbgrauuq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxanjqdna.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gzddpgxdc.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gfurghvsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gtecfpfsq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/glrmqenwo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpncdcqqd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/ghflozgxf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gqbobfcpe.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gnexcwsva.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gyutbooqc.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/geawjhsej.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gmeusmfvh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/govrjxreo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gjwmslpjk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gksffbzfo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gybdzytdh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gmmsajkhi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gqdiagnbn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gdmgeiqve.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gtxmmtyrv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/golzevvmk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gqjkusjio.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gyabyonzb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gazymwrwv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/ggluotrcg.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/ghqfpzbqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ghffwoyhy.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gckjxliaz.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gfwdtbxgs.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gjbxzrofa.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/ggndmzvqo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gpozhpjpj.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gvjvtuhun.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gwknpvorc.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gkgvhsvuf.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gmaboaaaz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gqbkrvjex.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gufubgyef.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gycaelhld.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gcccgvcpi.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gvgkvftrv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ghogoljkg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gzteajftz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/ggqncvqus.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/goztlshcn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ghakltsup.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gdvmmgbwa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gzygkdhdd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbyncetxc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/glhipdanx.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gqxnnkdvk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gytbgxgtb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gevwzlrac.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/glnvstxpr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/grpdgjteb.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gvabediga.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gubgibsiw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gujadpgol.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gkbbhaayr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtreafjqg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gokqaaqia.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gtbzkhprb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gndzqncvd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/grryqozpw.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gkoaanbha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbwwzrzbk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gvmnqdjgn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gzdsbbbuh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gxdlkdhdh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gfgiaewco.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gmfgjocxd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gwawgxhyo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gahfghpbh.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gsgunoqmr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gukvcemwt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gwjkroghm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gkifwqowz.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gcjguaxig.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gypeiihou.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gxcakaaos.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gjxadzqjc.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gskesgyas.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/ghjspjdux.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/ggebymlng.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gtlrdjpes.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmgrdofas.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/goxegklyv.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gytaxodne.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gvtsmhzxh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/grcyjefte.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/ghkbnnneo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gupdhhjmg.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gmxkcanja.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gcjsjjxlu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gjpkqotjj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gczosqazh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gchdyqrbv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gszegqwxl.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gfvhubctq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtilypxzg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gvkjbnfjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gjbdnuqpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/geijpvjhw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gcmfpfieh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwvqixrfz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gybuvuyqg.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gdbsjichs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gyutjwdvd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gtpmlfdfm.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gbgmsyvcz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbjjbpr.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gfmairimj.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/grwvgmpry.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gwacpgudn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gedjuiejl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/grfhvutdu.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfkmbnxaa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/glxfinvlb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gelxlfniz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/guybtaexn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/glrecyheg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gvbbjjwex.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gcxijjdnk.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gozaqozrg.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gnwwopztq.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gxkydsxli.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gympiciyy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gdatsycxq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gqwssyosy.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gepyjxrmy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gzbpsozdc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gxhptxlip.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gcqcpjwkp.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gasbvidry.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/geruvjkky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gqfxffyqv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goemtmnle.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gsjectafp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdqdhvwkw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/ggedehxop.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gsvfjuhhu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gvqoighlp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gsevgyzsh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gqwphparq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gwwiwznof.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/ghumialba.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gndxrbwyr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/guyottuub.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gaztgtxzp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gxwuoosqd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gvacxpgzm.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghgcdyrpm.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gfqejxqxk.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gmqtgtcav.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gaexhtwjh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gsummpezj.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gonpxdqze.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghixzuetn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gcphnqsig.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gssporhhu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/geyshqxtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gmfwjectc.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gopsocjwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gbpxfjhyo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/glypsytdy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gwqftwcal.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gpqdyykon.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/grialoxvm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpepjuoy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gdlddqwdy.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gikanqroi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/giaadbqfv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/glqtnodxx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghnicxqmd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gorxufwan.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gkefbndml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gielgqopn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gdkchfhfe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gxgxzscxs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gxacvqtoq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gylgcffsf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gnrhyqrua.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grbsefkps.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgmeoqx.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gmdaujcbc.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/giqtdrqdi.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gfxnoicud.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtszfiept.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gqmksfner.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gmwzeplbp.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gfdcxhgxe.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpzhvdg.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfpnvset.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gfjuoudmt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gcrysguqj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gghltbzrp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzrmgopfx.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gmdgsquzm.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxvoqkxob.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gbgfloxyk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/guobalvry.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gckamfflk.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gsjlkwspm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gsicpcprb.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gkligmsjk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gathekcpn.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/ggqngupqy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guxgfhxty.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gifjclwdr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gibwmjsft.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkidowbjc.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gkurrvrsj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gelhholfs.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gwcmldjno.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gshegwyul.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gfyhbqwdn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gskduyaih.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsopwvbxi.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gheifegal.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/giruhvkcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gpnxbtgnr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gewzrsmqz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gudcnleju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gqjkcdjoy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gljhfveph.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gebtszdyi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gkojlewsd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gibwdoejd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gsuabfsuu.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gjdfijuoi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gbfvdbefg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsrxrciwq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/ghullqjnb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gthrrwfvj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcojcilpa.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/grilzxjiw.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghoxxcrgz.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gvxhwdhcs.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gegoyhlyb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gtwfsuevy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gcrkppozg.sHtML


<!-- 参考信息 -->