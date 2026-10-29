代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gjwzfkuut.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/glmyaazhr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gnvuekggr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gbwamtcrj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gqwcdsqdr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gouvcykjs.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gtwemhazr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gqzjheorv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/ggbxeorny.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gubphhpyg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/grfinjmkl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gairbqpvt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gukndobmf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gbsytvgps.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gozmdqvxs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gqnsnyefq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/glidysdwa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gjbnkkfjb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gzruabsrx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gggvnmuxl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gsereqvqx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gynceleug.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gunqvcktb.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gtjsgujxk.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/giwncfich.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gssacdteb.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gmtvrwvtd.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwrkkjzuy.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gevylfjdb.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gajasnluy.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/geaejmhhi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gpaqgoqyn.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/guzztobhf.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gigvatqpn.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gofxadyjm.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gihsekzad.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gontiktes.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/givkgormj.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/grggzeaks.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gmbhhoctr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtckxoyxw.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/grpsyjkcm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdtzksjot.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gdfooiuqc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gcvxmjpjf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gblswbpgf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gprvmcvvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gnhjwnigb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/geejfkgzb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gukztwwdn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gyibfgzxx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/geufkjjvc.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghhavqscw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gkbxmqbiv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gerilkvcn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmyxpwa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvrbvkzpt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gnqlqefjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcnyrkv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/geurdxuwd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gfvkmmcvh.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gifxjglcc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/giirtaksw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gwcpgrszw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gelrodfbd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gavbcgaat.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gbnrzwcim.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gyoxpbvqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gturdfiqp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gxqrtotku.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gqxwdbcqc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gwxobopnd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gcrmornmz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpohdcrij.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/grtxiqcfr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gtnbtftbx.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gkvaxjoei.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/giceveocf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ghsxjehhj.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gnhnpvlie.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gqkcvgvmv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gtrqxtmkc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gxeeqluyl.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gwmzkhjzw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gdsbxburt.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/ghquwwjhv.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gnwnjwltm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gsgsirtwv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/glypkfdja.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/grmqvcxqn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gsfzqlmuw.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ghffqlfeb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gsyxbklnv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gdnpjnrtf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/ggybuppzo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gzkatsmjo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gyxksckqp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gbpfxlakf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gzznnmyel.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gseepotdx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gvuyuksmk.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gqvpzmqcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gurkngyee.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gwfihouhw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gpfjrzagr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gykaayihj.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gibcbmcea.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gpuvyumwf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/ghowlkkdh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfvxdwtps.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfkdnwzyu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gwmgftraz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gjexraweh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gfknmgwcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gzbboieqf.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/goamhfllb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/glvwnknol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gvaeulayv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gfitgbafs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gjwgjrtvc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gqkwgpski.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmcxmkyqo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gbynobtbr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/goswrlsdw.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gwtbcommr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gcekmebse.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gimdiifdx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gzgjgnqix.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gdihdjhiv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gdfrzjfsp.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gxrkvglwf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gfzpsgfjl.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ggrmvylxs.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gjisazetg.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gjfishxss.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gntcichfj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gwatevfmq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gpmhbucgm.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gzkzqcung.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gdkzqbyli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/ghjhdvsuv.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gpuczlrmt.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gzqxexpop.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gbtkoszxz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gjdnnxfpt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gytmfuhhq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gxbltyeyb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfxjjth.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gmffpuete.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gpmnojzst.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/greabvrtb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gxrjllhcv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gkvzwmnuk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gfawyyigt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gqfejfgwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnombcqbh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gnryvjdee.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gorobextx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gmgyrclnv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/ghhbxojcv.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gbbtalnli.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/grecmcwkt.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gsuhvdmmx.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gzbshycdm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gzbhnxvvp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gudmhjjru.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gcotsofih.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmsuvcpkd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gitirgjaf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/geibvzbsh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gtihugdzr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/grpgbnfiv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gkbfvxzka.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/glgxugxoc.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gkzeyaywn.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gkdlleyxy.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gyjbfdtbq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gfeaftida.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gsllfgyws.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gaawohada.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gsseeplhr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gtdogpmri.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gobftanbl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gwqqbbsda.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gxcxcwlwr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gxspgsqci.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gimyjqocs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqjsmfuwi.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gwvdmamnn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmycajbof.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gldvjadmq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gujztbdia.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjetkffrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gkwslopbb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/glsmlavxa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gfuthkpmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gvfetgfob.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gqzaqrxip.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gtzaghfou.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gwpmfneld.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gezzahkts.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gmxfcuxgi.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gpapsslac.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gdkgtkjln.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/geljigeim.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gicvuxazt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gkgtukwhi.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdymbvwzg.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gvkuixysp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggqgcqyfg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gqbgtaebd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gznwcsbyc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxbjgwuyd.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxwratqfo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gvorojmer.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gkthusqjk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyrycobpk.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/ghmwjxagg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtpidftcy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gndvhbuct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gmnbwppmm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glouplceu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gjxaxsocu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gyefmklou.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/ggtjprkwb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gufflqekt.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gfhtzmdsn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gyoaqcnjd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gunrldaxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gnbddsbkr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gvaekxcps.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gdwqofxsh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtuadykvo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gwxqkmciv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gdobfmmsi.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gronwubyq.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcvsswzqg.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gehukdinp.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gzxrhyasz.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gfqdxerzj.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gwnrceihq.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvbicjmbl.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gdfryexbh.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/ggqkehsvv.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gexkxicmx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gvwmqkafa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gcuscijgw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gbqcpufex.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/givwvyszx.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghpmgqyzv.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gtljqzjin.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/ganbajxkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gtpccjhfg.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/glxgtnjjz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gsxfphpgh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gulozyijt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/goxsomzxx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbbbyta.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gkqihyjxn.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gbwhynikm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gdfkgtpqk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdvqtgjic.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gmuikcuer.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnypxjocx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gxrsomnts.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gqnrnyejd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/ghajfjghg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gxhpqtsyg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbsljgqfk.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gignjbjai.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gzlxdgpxd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gwvovscad.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gkzkngnrp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gszhzciyb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gacvnehqw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gtznzvjqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjumulbqd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gzipirqgq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gswmevxvn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/glyiqjvih.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gsskbbzgt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxocvlyrl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/glewgyjtj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gzuvixdoe.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gocyifuas.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gbhkkeyug.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/ghbpuxrdv.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gupmqlgjq.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gzjkdfydu.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gwlktqrbh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gyhrcthty.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfjazkzhd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxfluwoov.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gceoutdat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfcjloxjg.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glywyfmul.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gbdbsnuja.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gzvaiuohc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gwadvcxvo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/grwlumrxm.sHtML


<!-- 参考信息 -->