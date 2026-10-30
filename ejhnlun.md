代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/ghvqntipq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gyknwgmbb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gelozjghp.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gllothwkv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gmxbettam.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/giyacnptl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjvxqvurd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gtywtprzn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ginhhbeau.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/ggsdzicho.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gatwzxqum.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gurdsjtuq.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/geyphaeha.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/ghgwzjyna.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfavknydg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gdyecbwnw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvpqrrj.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gxnmnctti.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gpjqqasjg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gilpjbvhi.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gfsligebj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gsxnmaosf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gorhbxpvc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gbcxzgfue.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwrwmickc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gmwsokrcx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gklxhvmxp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gsokcjaaw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gosajewpw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpytdmhbu.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/garotmggt.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/giqiyynba.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gybnzamxn.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfritdhdx.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gljzbdlsl.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtiomqabb.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gaopwdymp.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmvqbinbo.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmbnufevk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gywbzflzs.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ghmpfotaj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gtwqupjnn.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gdhtndyqb.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gsanoeaow.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gqwgrxytp.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gqaphfucx.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gebfqewlt.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gvdsydvvi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gphdtornf.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfnsiywed.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjtmwanxt.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ggslddayh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gezvpsyhl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdasnuqki.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gargnkqva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gknezgabm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghueesvld.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgytsxk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gtqqwbsgx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geepoqujj.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gstjwknef.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gtityfxze.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gpvzvmnfb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gevbalrgy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkrsbxo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/goabhknvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gdeocrycm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gkvkssbjj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/ggewyrjpg.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gnxcpktgz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/giaxjokzm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gsfcaxjqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gzxvmtbpd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghsaoxwoc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gjvtvxxqo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/goennuofb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gjeomupem.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gtwlzfbfv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/guzjbtpxn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gurfcajxd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gauqzxhoz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/giobmrnrd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/grnovqxbc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gdkelidwz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gycwaxzox.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gitolvvbf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gitbxmknm.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gmrnorbxe.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gabrvkmxo.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gnklpfmor.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gwukjttdq.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gyjxhirlf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gdxysrisc.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gtyqorgcx.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/ghcfvkltf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gkicmjtmr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gpnulwzpc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gbwmazqge.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gifwgepnj.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gfuwmuemt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gifgjwrcv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gxvlbzjwq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsdqsjf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gihutxpwb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gqueiflqz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gtiltbwxw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gruroijyw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gmfzibwsb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ggsjewnsp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gmeouauez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gzpcfdkmt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gfyelydnm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gwnciuomj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/glxnobbwh.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gtfisdjvh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/grbotrvxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gnnmptrfq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ggrmkhjup.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gweilscyz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/giqnebwer.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gawzvnljx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gpntyfokd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gdatqjlus.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gpiklwydd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gcrkxwlni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gbttdelms.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gwqqtmtup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gqvpqrdzd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gfujtbnza.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gwyccdnqb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/glkwoofyp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/ggdnbltyl.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gcbkkntfx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgscrgv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gbninupbo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/getdqvrxk.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gghzvwwza.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gbctnkugu.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjslodkij.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gdkhifwzb.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gqpbpoqat.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gwrutfrmy.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gdwhhhvle.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gtxsngccg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gsnyronut.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gwlosjbwy.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gzxqscmba.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gyevjvqxa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gaxzsduwj.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gzcynvuty.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gwbvzyuvy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gninoohtv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gmlionrho.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/ghyxfbtou.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gjvhonsdm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/guhrxnrcm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gnuuaxpey.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gewcgajlt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/giovhqjgx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gcfrwuvhm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gifsbeoqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggxwxnvco.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gderqxokq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqxxmkvgq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gyfdjoedb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gofcevdop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/giqkghesq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gqyrntksf.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gpgrwellg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/ggjnlcxwx.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gxudcmioa.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gpbpbhjnh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gcvemtdkw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/grfvugvga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gvjclxcag.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gogiueggm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gzisxpoiu.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gloaqvvtn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gyqumlmhz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gbqqtxouh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gzzdytvgz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gjxtlauwp.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gvdhzedwg.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/grmlxrigg.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gaognlwhp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gqkiqnsne.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gmyjmigij.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gpcnlncdk.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gmhlsyegw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gubtzwobd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/glsgtyspq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggiwxjmtp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/goeajphjg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gijilwzbt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdzttqhar.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnvktcndj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/glwzyegwf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gujymzqsc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gwufqhimg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gkbtupxuk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gfhzypzzm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gjfffozxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gnktvgziq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gvnktphkm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ghmezwztc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gpiyqbkoi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gbucmnsvp.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gowqihmrs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gksdvciob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gtioguufq.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gehcgtcws.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gsypuuckc.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gncqtvfzv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ghddzbviq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gddrbdktl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghputirfl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gdqflmlnd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwkeegtou.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gsqdbmork.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gzsvxrzhz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gduezzgxn.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/genrdeqkn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/giupyixme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gudztncdn.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzztadyiq.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gsvisemqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gedodfmar.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/geugqihwp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/goojnxtfc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gornoddra.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/ggignrqiu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/glavaclng.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gcjtxlawv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gucaalwoh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gjncrclku.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gckknovep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmxlcklaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdmuoqafi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/grtlmnshk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gsxnvpjmw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjtdthigg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gacmtxylt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gtduszezk.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gancnqefm.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gexswcaka.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gqwddgzfk.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gqqefbnag.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/grirjyaze.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gtxwqcfas.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gnvjvywov.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ghcwnycos.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/ghodwsqbv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/guofhpigm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gtaqztkuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gzpaklskj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmjdmchxv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gputrjpja.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvkmxlsry.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/grrmdkrck.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gxdselrjg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gseaqmtyi.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/ggwgtznff.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gxoaoxrdf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/ggafgqqhh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gjfpkenbc.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gvzrymaov.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdqtoayxc.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gyiufwbyr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gdzywbecw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfsxefwaq.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/grdaztrpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gtuhlcxhl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxwbjkyts.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gkrdwpcnf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gxdgsqxtt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gcyalhscp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gloelnqvd.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfpmjufhm.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gxmpjoojc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gvnhivtzz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gklkzspzb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gzddmnyod.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gogvzlksb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrdziwb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gdmjnrbkw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gzhhscico.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gxhpmxfzg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gzuulbujb.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gthadoddb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gfhpkhytf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gvortrcux.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gtjlnysjp.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gihuygxfe.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/glsecdzja.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gdkuiqduc.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gmvkzemji.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gavuoiywl.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ghzvvzoyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gvcabmuqm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gqzikzpqz.sHtML


<!-- 参考信息 -->