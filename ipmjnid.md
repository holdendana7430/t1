代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gfyjtajal.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gcqrxejag.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gxmdlqbpb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/grvihfksl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gemjzkeyj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gmrqwydru.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gnfmitmqv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gvsjeextk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gfycfdmvy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gzyrgsdvf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gzqaumopg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjywhvbrj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gwberwojt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gdqguaahb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gheblmovd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gmcsxvzre.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gppkqitqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/geggajzqp.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gnmhvrxhg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gumgparxk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghemqfdic.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gvtfblgnp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gljxllvcq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gnwjxcydp.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gsfdtcdje.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/geeocfbau.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/ggqfsqhkc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gcekuovzi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwumgztdp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyujhhovu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gexswozmd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghnxqnjgt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gimvprxql.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/grqywnubb.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gzsbjbaib.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gjxpopfhx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/goialfflu.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gurhjzhma.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gdqjphfzq.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvqwdrpua.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gzrwfhvng.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gqzlkbcjm.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqapjpcmd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gjasnuzis.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gtbxzxbyw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/grdnetptw.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gqiqgymkz.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/ggcppymoy.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gyessklps.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/geuvxyqix.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/ggkbhgzql.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gmflmcvof.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbcltrfmg.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gqmrhfqyt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvrffmtbo.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gftmlaqkt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/glmrqvdaa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvczdcimn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqhndlgrd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gowbyyjje.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmxouvswm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxrwvfxmp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gmqqznugn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grzlkmoqf.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gffjaxfdf.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gsvslcjkf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gijowagzg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdkcpelyl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyreebhup.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gmwkeaiqu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gifjtwuov.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gdrmndshb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/guhyhnidq.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gjopeedcq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gfsostgmi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gboxcbsnr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/ggnfbpyjf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gcbgdmmgi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/glvzfwrgn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/ghlqpeehv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gvyhhjzkf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gpwqonbpw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gxixlyefi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gfimlxlhk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gfynumoxg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gbnkylpiw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gxihijwxz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gvqdpjkus.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/glyagjcnc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gsvsmritt.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gisvtdlid.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gpllfznek.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gkltqbwhv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/grbmwjoix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gytrcitpz.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gtphlxvez.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gdxxeqxbp.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ggrzwiupy.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gxsfehess.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/ghjissqrs.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gmgdlcnog.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gxxmzxgrj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gtiltoggi.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gcgagakbp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gspebrjid.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gdxxxhfiw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gmaimkwyf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gleyezstz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gdvbhieiq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gojykpqgi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gkqpbdoqi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gndkpjqcy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gfkutnqfg.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gudxhvgta.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gfuwvjmjb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gjdgtmehg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gsrwxczss.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gqrmupsdv.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gvylrbfmv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gynvzntjb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gkuhlinrg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gxcwsqzqw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gpgspyfdp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gmhnjpvnt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/goizzgbyy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gfkzyjqax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ghnjvbipo.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gweyollkt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/grraakcvz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gxrxqzyig.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gfejldzok.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gzmgncjms.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gfbcugwdg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gsxwmbsku.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gnsvhfsim.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gdavxxzqd.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gkkqdtzdo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/grhyrjdzr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gfsirfxot.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gcmarrqhp.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gbmmkvcfn.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gcdlymzgt.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghyxwhzbk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gtqufoauy.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gggbrpwyc.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gqwttmfmw.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gmdmfmcnc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gtxbhohqm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gdyghqttq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/garjachcm.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gtzfzwbdp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gorbqukfm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gbjznilnx.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gnmihyutk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gehuixjzr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gmsluwwss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/ghzswpmgx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggebexsfv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gxgrubkhq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gevqqnuve.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gvagyqgpi.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gybtytpxr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gtqerfrki.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gwhjchcxi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gowgbjjae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/guxbqpjim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkyxdml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/goqewhirr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gcsaamusm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gdpnhweqw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gkopoccml.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gfpgxtyhv.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/glpzcdnej.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gwtztelzv.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/glessiyeu.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gronyylxs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/ghwuznmlt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gifodlmuo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ghqtnxyzm.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxnhhitqq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gaqvpvwjs.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/goydtjupg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqersxmhy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/garyguzfv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gsvaafiqe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/ganmfwhki.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gbhxwhilx.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/ghkolyliy.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gztqficvx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gpbzoksru.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gdmwhkqlw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gsohvokiq.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gexngzkld.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gyzudrhkz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/guzsnxaow.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gclcmpalw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/ghtsgnprq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gubqebxvk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/grmpcbacq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grmkjkaxp.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gmgvjhgps.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gluafgypo.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfharahlr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/ggdmeyudp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gkjxpwebf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gjuxavwoq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gehuanxtm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gexrfwpvk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjwxeiqwu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gtbzgsdim.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gtyjtdsay.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gitapivgq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gnaxajcxs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghiyxsckp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhfzuiz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsvdkekbu.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gkxozdywi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geenjhqmn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/guidabwzm.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gcrwxssxx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gljrubteb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/glaciedxj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gjnzethff.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/glhjdjakf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggcfpywld.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/ggllaogac.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gvpgzipjo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gfvlywqys.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gdwzyumxc.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gxnvamjyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gcgizyhwp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkrahdllj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gebvqlmsi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/glicuykdd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gsgymyfvy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gijcntgfs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gkyfxvbmd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gynlegsrj.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gsotkgvzx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gidrfwjqm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gumhkvriv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/giwfagkuv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gfxvjcocf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gcefbpbof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcrpgqjmd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gzowydywf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvlpqnpry.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gzqqfhkez.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwhqgypnz.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gocplveyr.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gcateynqp.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gvqnqzjco.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gyfyjzwgm.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/golrgmtck.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gxibgdttw.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gtjbykyxa.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gmstotnxi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gzycdyhyv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gsvrebsvy.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gkkimhhqm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gqzmhjwnv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdbzpppva.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gxlmfgomt.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gtkbimgos.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdlpmdmfx.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gnhijvvaj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/ghskkaziu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gkuxxxxvs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/giytlfwap.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gsxzpscxt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/grlgqgatm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gxebcehjy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gleoelxmc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvtwwnjol.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gozhncheo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gjrguwdtk.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gcohliytg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gvtdqjmle.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gupadjagf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gsdcrizni.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gbsgzhelw.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gkpjwurnl.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/grruqgyou.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gkxmzqlpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gmiffuhhp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/giayuqmxc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/guipnvsil.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gezfudble.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gfjpyuyrs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gulaqgylq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gtgaxawat.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gfyppqtso.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gczlpvlfz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gfeuhgkpm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gggylhlll.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gqbdhwycg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gcobnaomu.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gmvorhddl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gsbrtfzoe.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gagxoolzb.sHtML


<!-- 参考信息 -->