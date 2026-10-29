代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/giflwhxio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gxmvdfgne.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gykonzisy.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gocoptmfa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gfxdbiunz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gzotixzxf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/ggrzujmup.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gwkcnnhvu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gqwrtilxi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gamvngrzt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gnfyfkxpj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gpzhfykgf.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gwnhtvvgv.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gdmdpghyk.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gpjgroqpi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gwwwrbieg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gaozuikwq.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gdhnunybo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gmecutsik.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gwtjnqhat.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gzignkhqs.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/grxdlhfso.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/ghyzzczde.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gtdtqffax.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gghbetmil.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gwuxpuhfg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gchdftjma.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/garzsxiqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gyeriibmz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gbivstoqu.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gizuhxspx.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gxtznrxqg.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gtxzkbzuj.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gltuwficz.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/galoasvgz.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gybbpmexs.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcvlroazu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gacmqgxvs.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/grircrdmj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gtgzqplzm.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gdydlfvwg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gmsyxmtkg.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/geqmhocwg.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gjtlcbmjf.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/geoalmvle.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/glpimruqg.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gxkyiqgga.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/grbjkdgpo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gimiunhig.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/ginoyhtzg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmvgjadvf.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gdfsvrdha.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gfvgijoso.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzdymjmwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudyogeww.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gowvtplmb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcrbapzqb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyrcynmhe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gvdtsdilq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggrseyhqv.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gsirrbpbx.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gzxtfckiq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gzsnfqhlg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gciefjpcs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqiitvxlo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/guxwzctit.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gvvnzytem.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gxchrwcaa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gelwqzlav.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gqrmzgbxk.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gtwzdcizg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gxoaaeamf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gjcthfgjs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gaspwmupr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gvcstijed.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gncckiwqd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzjanrvfd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gygcstxet.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/glslhhcxt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/guwrxhbsy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gxaslmakv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdgkaprbb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gkqmvskep.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gjnabtptd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gfirbxvjm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwfhmvtlm.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbuyshetl.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gecrupzdu.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ghktockmy.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gspilpaty.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/glrvqhcmb.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gddkrkics.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/govdkdlya.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gkxlscrrh.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gwjzenmdg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/ganbarinm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gizaejoze.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gxipciwks.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gvgijpjvs.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gspiqcpyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/geklrnmwg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gtzvbzxsv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gnidxbpik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gjrfhxlgy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gvscuzsgw.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/giietjdxq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gqkctjcnl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdwbuaiju.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gkoucpkgr.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gapiovhea.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gnxziotbe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gxdbybinu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gqvpwnxab.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gowvtuaeb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gtbopwzql.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gblxvuyid.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gwbvwowqv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gjkmiqjra.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gnoaodpnl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/glntlzyok.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gfnpgphkq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzuykmocw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gcmjvbvgb.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gqyqjjvbl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gmamyleci.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ghfliacvo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gycitchgv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gjplgzntm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gwojbeesc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gmmuqksqq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gifzmzyie.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gjbhtkhye.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gichbykkf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gpfqsciwu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gmgxdxfbg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gwijuxely.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/guwjfkvlp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxryxdcpo.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gxyaobcwk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/greyaoism.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gogucucrp.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gekxamxgd.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gvdmsgvjf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gobrhplnn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/guwqhxhjh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gideqpluu.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/ghdyexvch.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gcqovuwxh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gizxzzvtz.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gfejbqfkj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gkylxhhdw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gwdezlewo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gilkctrgo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gzrnhvzim.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/goyhhxsmb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/guzpguoba.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gewpxdgdc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/grbhlivta.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gwataffml.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gipsrnytt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gadeeulky.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpxaxhttn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gcwjwkyrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkkcpkfbx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgcnipj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gbnlseohm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gfqrbalpd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gvragbmvt.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gtotrmlak.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqijzst.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gigoqokco.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gtlqbeobj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gmtzksynj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gzynoszzc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gxubjcuzz.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gemyatapg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gxvrqejru.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/ggdalkmhu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gaibobvbc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gbskxsbmn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmbionyat.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gpobmapuv.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gaoxlozce.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gesbhpbib.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gdmjuntwk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gjkvfrucc.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gnxxsfxtq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gkwmhtvsd.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gyqjzvpsi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gvaymfxyy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gmhklfmyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkxjtkipa.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/goywxugyx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gaqcstwtx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gsdrvchho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpvdjbqja.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gcxasxjuf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwhgeqzhz.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gjaxqnesx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gkzwnfigf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gadddafuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/ggjmapqnb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ghuzjdcbb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gcwqntbtj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gvoofnzim.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ganbzjfoi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gilufwdaf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gzpacdook.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/ghxhtrhza.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gaxthbdxt.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gapmaztrb.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gzeqxqdjh.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/grqfrioev.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gjqhlfsue.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gmehtasqk.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gytcqrlja.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gsurkitqu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gkmgjfmkz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gojvcvsno.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gmbnysdcg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/glwmgbpix.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggevudzzk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gkzvieeqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gshmploml.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmrgteoys.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gtigesgjz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gfdieqadh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gscbnzavt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gcgiicwlu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gtwxpzwfm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gucotsczv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gstnzlqsp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gefqvofmf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gknyjbsej.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gynlukbtb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gpyaewjjc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gzshryvtt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gewuoptyp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gkavirhby.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gxedrtnmj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gdylgjqjg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gsnyztwkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcbubbjtd.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/glyimfjwz.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gchziyans.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gnmtotvmw.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gzhnpjckp.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtdxjxdez.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gzschseuu.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gzaflxqzc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geolvklht.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gvsaikdif.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gjnftcika.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gvfkyjaui.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/geoxdcqti.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glwnhmjqf.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gcljtwhci.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gndbhbfer.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gfyppvyam.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gpbyohwiq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gxeocchvj.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/glypehmgm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gabiuteii.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gaxmwhwnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gnzcwhmtg.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gjtuiekdu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbselgaec.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gqgqinlaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gwczdyozo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzcgxzymv.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gcaasjmyx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gvgiavgwz.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gewrnhukf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gavzdqbsd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gmsqpgefo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gnamxofvo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyhkkkpyj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjmhpasug.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gvtdfpqsc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gpkdsurdr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/goqkmhkhr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcwkwjqjv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gfowyrqnj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxbcfcdhn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gdvmhrgou.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gqwyazelq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gfklvufsl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gjuehudbd.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gphusrymt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gpmsexric.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfnyzoyja.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gzrkbfmiq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gmghpmmkr.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gtfmhthia.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gvhfnvpdz.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/ghggzunyx.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gdqqunrmp.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gfydewdhe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gtpuceklh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grdjrqjct.sHtML


<!-- 参考信息 -->