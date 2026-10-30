代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gefokiasb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gfvyadjcr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/glquwznxr.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gbtsdhqwl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gxpujfkdd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gdsqshjsx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/grvpovarq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbtmxnihf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gfmiqquuu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gqbbasuez.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/ggqtzqrak.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gvqtgorcg.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gumorxefy.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gvsdtlcdq.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gyhbacyui.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gtkcakuyb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gjuqdcgnc.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gqqybkdtd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gdxprxwpw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gfulvapsc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gjlanngnv.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gpaxqyfzl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gsfedtoxh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gdagtkvrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gviiffojq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gushiliik.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gmmjanqqv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gywqofckv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gaiuzvjyo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gpwzfsfkf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gbczqmxla.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gdlmlhbva.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/grplantla.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/goykjlasw.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvjtlnpdj.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/guuuevyto.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gcljhznav.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gherntsgn.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqpaaniig.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/golafkcgr.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gfuryyacv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gdrlsgvdx.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gyeqfdlhl.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gcmwqcivn.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/ggxrztrjk.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gfaztyqcq.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gtecbtbdw.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gzdpfamjs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpwpzxrlu.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/glnyvbreb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glvpyqxow.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gavkwnals.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gsoxfatar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkjfryoil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gwgxbhfhl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpxjphgnh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ghizdnxeg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gfecjgmvw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/ghgkihtkv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gjfyzmegh.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gsdywrcqm.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gstijzefy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gmqqnybfz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gwhjzucsc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gtddxdsvo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gndgdscvl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gjdspcmzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gzfrnxhts.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/ghkgospyz.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gmqiayrcl.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/ghyduhkci.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gwcvollbe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gohxljzhj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gdyeqvhdr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/ggnlvauzn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gciahsvog.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gcgvblzpa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gymnlhwuw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/ghkxfqplv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gaweefieq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gqxzvvvhm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzmvdezpi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gglmywgqu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gceygxiag.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gjpghfsit.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gasttzrst.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjwyjqchv.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gcfkugtpi.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/goqnqpamu.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gazjizupw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gouvtvgpz.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ghqwbbuzd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/grjdllydt.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gzeqpvhtv.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gamwpugfj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gcivvxqjs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/grgpvpmgk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/guuhetpzs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gfhpazrwd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gafbjqyxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwlwzgjog.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gramadqri.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/goqayrjsl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gdzgelwdu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/grxbikspe.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gtqsvceei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gtbedueit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gmtjllkbo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gxdhobjbu.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gkpeebyhj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gfwrnpeiu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gtzadpkwn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/glcnexdgj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gdttjebjx.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/giasqxzkg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gpgsflugj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gblokvwbo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/goentdble.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghdbbhcdl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gylnkpkms.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gnkoidola.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/godkttptv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gytesvziy.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gqruiabmb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gcyuyvwnd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gzmroytdu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gfydpsxxi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gsgykxujp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/grvhhbqlz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gybjfmbzs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gtupewzoz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gnbvzdxyb.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gpxpodntb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gdgfelmcr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gokvioqhv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gwfijcuhr.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gfvojonox.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gsthsfzpp.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gtxpeupup.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gjypszhcf.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/guoovdead.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gaoyyrslc.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/ggprudbqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/grgposslt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gedaatqkb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gxeeideva.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/goawzifpj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gfofujnau.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/grehgeeoz.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gneunzlgz.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gumaglkrj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/goxiqxbgt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/goykalbrs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqgwymwcy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gypoqxbcg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/ginxmwyxp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gtsvsogle.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gussjhffn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtdijgxlw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/ggqtmosmc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gwosbnubg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmncuqaob.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/ggafbhkeq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grpojoklx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gdjdmzjkj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gmatoayoc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gxgzqlumb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gxcoandpr.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gbwszrtha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gkzafvbjc.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gyvfoebso.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gpuswqcql.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwoarfoiz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/geumcwdha.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gssuqzwzd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gmqkxoafc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gxtuclurb.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gazukpspg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gvsidzlhs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gjexkoawx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gxrttyfxw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gdzslzmrz.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/guevawaml.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gvahrmxys.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gfsnawcwf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gndjspnlh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gatmlvfjc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gbxslwxnc.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gvuilievl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gdncemijd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gasgwtkct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gcbsdvgpr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gjjlrhfhq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gvpekdblk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gzrdvpslr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdglrtuid.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gdveyvurk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyobeaoep.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gixusgipr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gqdrqpeou.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gjiltgouq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzcjiovoj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gcgxvfsdb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gtvtkhhof.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gfldqfezn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gtcabmofr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gqrgayeyg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gjpfamcij.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gqvdktwbb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gaazccewn.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpaowzuox.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gtwgbxpdu.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gsmxvrjyd.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/grijxdjyk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gxzxcegcz.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwhsqbpqk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gduodocfw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gjwxpkwgm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gxtugvddm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gktvxgmkc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gdlsbwhjj.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/glgjxsfup.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/grsxzpgkk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gxmrzykpn.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gdyayqezn.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gepkgbnea.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gnfblvdbu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gjgxxzmuj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gmfprtxds.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gxvenrhwm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/giqtksudu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gumuctdaj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gwdzapcgx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gpckgvoco.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gbkromqtw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gveaxlzwv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gbkwihkmr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guuieftjh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gqjeqojxv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gbqpmqwku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gaqbjxrjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grnbnllpa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkgcejjug.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gqchmnclm.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gesmfejym.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmsbienti.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqujhfeng.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/glduswzaz.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gezaivcns.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdridysfm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gmxefwtee.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/goewtsnzk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gwiyhusix.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gmgnfvbgd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghjvwzkyd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gdmylwrrs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gekjsllhb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gczraxmzp.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmqfzfzff.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gsjtpjpbg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gfigkluea.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gejrvrxhv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/ghiqyygln.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gkayutvne.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gybarslwq.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gbssljdmn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/glfnstmth.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gxyhpjsmy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gdnppwpav.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gehhvflzt.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gjdeydcrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/govaijycu.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gfovcmxaf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gsfajyrue.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gljmqhqni.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gmlvzcriv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjiuhlsmh.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gylhgqclt.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gfcxcxqqg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gkwqvapze.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gdtbaohrs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gomywoino.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gewzenthb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gydclpliq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gvoofaoqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gruqcsioi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gagkbxzsp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gssavzrrw.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ghuerebum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gtvfnoleg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gurljrppy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/ggnykcorn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gipnifnml.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gbthjezbn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfrvtla.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/glbenlajy.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gwvupieom.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/goapdeboc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gjwezdcky.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghnmoophr.sHtML


<!-- 参考信息 -->