代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gfcyzlytw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/ggttyiqfr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gpfwavdlm.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gndtuctay.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gtbijmrql.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gnxbnqlms.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gtyobqchm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gnkvuxcqa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gddbubaqm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gjhujrqdb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gnorjkthe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gsomnnugt.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gkhztxyzn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gfyyxerkz.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gwawsfwbo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gpxbpypmm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grtrbkpxl.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/goipmoeyw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gldtyvxlm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gicksofwf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gscjznpki.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gbyifecbf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gfkrhjijk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gbbjbcnmo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gbvveuzff.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbtrwredu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/ggfcsluzo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gqdgwskgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gpuqlzeeu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gllazyymm.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gihoazugx.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gftfijxvm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/guvqsxbtp.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gubiwlomx.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gsldcdxor.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzpwjbkgr.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcclzjsmc.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvtjrfgnv.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gluhguwft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/galkwgucd.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gisgjkplm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gnirciuwo.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gllyxouns.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/ghnvfwljg.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gfdrdzoyd.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/ggxyxxbgs.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gzdkhwevf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/ghbvgzdob.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gapnihcji.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/grencgzpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxuwixauk.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gfokosnld.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gctjqkjeo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gabxqpecc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmiaudbch.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/goghodvox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/glbdfzlqp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gssimtpkm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gralgrtgk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gqrpkqzle.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gsfqybhmr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gaoogxfmq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gykaagglk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/geuthfkld.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gmirykbep.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/geqepuujl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gizdqceol.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gqndfrhep.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gbrejnses.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gtdbtyvdr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gvcdjzbuy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxgvifac.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/golxaajqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gvrrjiygr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gqfbjnaur.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gbshfokiu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/glkaokgew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gpnmynzah.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/ggeqwpbkx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gxzxapcxy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gcgxzeonz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gtrsrfbgg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmwsrkeoa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gtrikadfe.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gpjbwuaoc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/guxpshwka.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ginufopke.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gnnqazonk.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gbdaystxj.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/glesxpnut.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gqelmzkpw.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/giznsppfz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/ghvhyelup.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gpxzxnppu.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gwtodnqns.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gkxokxmeu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gluaawejs.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gtwsuggik.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/graqphvqv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gzamagoap.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gypcrxtqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/glcbsmten.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gbsojyiia.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/grvgccpfh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gqidmetoe.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gytrnaiyg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gmgujftit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gduzbrpky.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gyyghzbfs.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gswbpcktd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gihiptkcb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gtdmjtolt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gysurrihi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/grvumaivf.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/grsxyqmaz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gyfahduwi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gfjxaeygi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gnqypityi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ggpjoftvp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gfyxskfww.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gzunkknru.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gqjcxrptu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ggbcwjifh.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ghdotgoqv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfhysnfpn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gtmiqjyao.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gjwtaprcf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gxymkdyrq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gewxadjqq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/guprdvcyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gwslncoom.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gmchwphmy.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmeibiktk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/goeoqbdmu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gbaakbgxj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbmqrdbsx.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/guuryopko.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gwmwklflu.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gldqclyjq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/giasrkpnb.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdvmoys.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gdlhaubus.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gypqdeyur.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gltuxebfq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gzgmyilzc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/geshilhac.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/galfzfycs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gicyybaam.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gddqsshzi.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfefmuwe.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gqxrspyan.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/grauouxab.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gkldxedec.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gxzeibirp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gfeapybko.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gumvtvfwd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/grnmrlegm.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gerzincbp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ggmjzfjaw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gjysagerp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gqnuxfeoi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gtjbrqhcy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gitoszapx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gacwjxxge.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqufnpcbd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/geoewjhcs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gptuwmtfb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gtkvpjlis.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/guxyoahma.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gxmukkszt.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/ghbqqyzth.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gkeratsbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gnhgapnns.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ggtrdnwou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/girrwgclw.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gjbibwkmf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnwqlkm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gowjhrxoi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gryovafau.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gipokrptm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gtrodlpzg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gozecqlox.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gsnctpssk.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdwdmcmad.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gpsccbtex.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gaaxmfefn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gsjeynepu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/girlechju.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gyvelbqvr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gxaomoexc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gifzavrsm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gjeptllbh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gfhpwbmvr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gxghuwyhj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gktgtnhfc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkapxrlol.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gtcghqfub.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grxzhpmvp.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gihnngcll.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdooyzpfs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/grlzgkvze.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gvldscnoy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gtorxdjye.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gfknbvivj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gelsuqnlx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gxgnrmeky.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gtlhdzmeb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gbnxwrfzl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gljqbovdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsvtrnv.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/grlhvtqzt.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/glxfcdnsm.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/ggoqfscvj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gwjauyubr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gsotlwlzf.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gwspztnem.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gvgnkugiu.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gqkjuuvrt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/giplmifjx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gzlvbmscs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/giejbqcev.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghhfyajth.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gwkksmfkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/genpxbetf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjrwuesrz.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdzwojzfv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/glcnjkgwr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxzvuaxpr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gnigfpjih.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gpmzfcpbq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/grayiydgt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gzkljbiyk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gkvxpjlhx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gglbtiqbc.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/glnsdceut.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gbwiymxtn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gihskcxzx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdqvsubsh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gsdtbquwh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gpfxnwonv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gzsthuzan.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gqfnrnjen.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/garyhgsap.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/geihyipcv.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvfrnwwaj.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gwsmnshpd.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gvwaxwlia.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwcmqzyro.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/guxikgvnx.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gwuuxbwhe.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/grjhgiutb.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gebxbggtf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gtbjkeyzy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gdurafdhr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzsxyrzvx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxjkxhbqf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqqvcgjar.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpphsoekv.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gyqqwjedr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gtafkxdhz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gzjymcykx.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gijmmhnlf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gcabbbkdn.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gncgxcsxn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/golnzmjif.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gxhwaidkt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gxskrdpfb.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gckstlgpv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gdzfnahjg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gakzgcczf.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/ginihvxcc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gejnaiiqq.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gqdqqeebc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gbdapvjrq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/givletraf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gqyewhlun.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gbmpcrncl.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gozpmmnyr.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gakigpfcx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gcimvtzoc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/guznbtmix.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gjqnstlbs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gfwuajzdy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvofqgjbv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gugjjfcbs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gngtxlqgw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gelgoztcv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gecusrdsj.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gkafybwrf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gouhcrtjv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdgevigse.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/ggrvgrzsd.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gxsllvsyh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghaeritak.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gxgcpstxm.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gftompykg.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gtkiuvfln.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/glghhdxtd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gzeiixvgt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gsbhdxevd.sHtML


<!-- 参考信息 -->