代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/ggsginyku.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gtkrcnfto.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gndokobob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gnnnmdawl.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gwlfmpbor.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gzckfowsz.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gbxquylyw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gpbnjyzqy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiggkid.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gvbmkgeco.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gfiezreph.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gkbuxywaz.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmmfttq.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/ggjhoeggt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/giahrsxhh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gaidnbscg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gunoomppg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gzcvusiti.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjuieezsl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gtespkbrh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gatpddhsc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gpbrxugzz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gdusvnith.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gewmpajag.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gmusmmfhu.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/glgyscjrd.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gybaxtafv.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghglcruab.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbdsighfz.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkkiysihz.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gaayplvzg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/ggqwfxkpc.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gvevvkbkq.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gjepnvqtc.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzqjukqlj.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gnvxrcybw.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gphgkoysj.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gklbxsxwb.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gbdihuucz.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gufjjvqat.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gluafzwoy.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gowkhcvdg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxorpnlpe.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbupvrhsv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gjkbyhxyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grrjsuqht.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gipgpupzk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpotkozpg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyeotasbg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gszqlyfih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/govfqiakx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmclvuquh.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gnuobjfdh.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/grjcqblmv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gaxoisalw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/ghkibfwgq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyqtulinw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gusjudxsq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gxhjejkbt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gnbqnsshe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/ggxincjqm.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gmhsroavb.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gdjusxnlf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gehycqxqo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gleexjxjz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gfblziapz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gisyywrpr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gkrniyloe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gjyuijdqh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gpyzlnxbs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gndnnoxwz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/ggomulquh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/glagvmuaf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gwicviisy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gqaxgamca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/ghlwwtfuj.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gyrxkognq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gqjaegiby.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gwxjrvlka.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gyuixsjpd.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/geusbgemm.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/ggmdcmtol.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gyaodpern.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghhjzuedn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gzqkqdxni.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gjpnccavx.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gfyvjbtgp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/grthryken.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gpaiybvlp.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/grrdruxkv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gfrnpgwdf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/ghzjulqfl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/guxhlljyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gdbospxwk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/ghrqnwcnb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gwktynido.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gijgcvoyt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gmlezwcbz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gmogowlau.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gmjuuebhz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gyjwdshlk.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gytagemuq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gggjipzzt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gowlopzpo.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gyqtzefjn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/guldwrnqv.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/ghjbjclss.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/goowgfmwt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gtbzppxip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmloxyvjx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gwcqbsleb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/girfpuskj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/geznvzuho.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/ghjhfjppz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gpukmznqu.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/ggmeehosk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gxqhbmbdu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gpdzkbcju.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gygysmznr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/ghscwhyvh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/giydpcsxw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gqdtxqfbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ghsnrksyg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/geiskyafu.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gavcppnfs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gswnghdah.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/grgzutirj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gqwsejiix.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gatvwjlge.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gabaxlfsc.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gihkvrjoz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gjqytnlhz.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gndsdaxrj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gnxlgwuau.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gmrzefqkr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/guhcxpndy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gihbzczvk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gvblfqcbw.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/grqxvvxct.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gxqvaocwz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gsirichji.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/glhdqxizq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gifxlumgf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gidnyoazi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/giqgntqtv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gfhxibbmd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggqrckeyv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gpuxdyczq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/geuryzbsr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gtujhgmqy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gkbspewcm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/girpdadwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/ggqlxgtlv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gwnstmyjs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gozzozldz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtxdqzkkf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gabgtyenn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gwwspunno.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gemogmrao.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gmykmkbho.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gffpokwkx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gijvpszom.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gvbrsewuj.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gbyvhqspa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gzsouxjdz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gneppdsta.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gcuhlejzb.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gwpiwccnt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gbfspddzl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gxlpztzaj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gjoyjfyqv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gnyxpnxnn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/ghjrzgile.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gcftahivl.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gupixdgoz.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/grmwsrnge.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gzsnmjthk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gploqlioz.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gtlgarmvm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gdneoifab.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gimodkujr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gdifqvpmu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gicmcnahg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gqfydeydk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gbyjdbrru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/glbejybcd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvueehftc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guubqkbbk.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gfmaeykrq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giotlmhah.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gbtxbgxxz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gdlrajamb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gtlpprybk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/growiufgv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gwoumnmeo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/guycbhrlj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gzkkbhhos.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gkpgcqesn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gottxvfiq.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gatzhmubz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gbjfaensa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gsvmrjgup.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvhsdtoos.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gxjonztex.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gnphuawrz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gblcxxalk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gyunujlfr.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gljyambpo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gqrradfju.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/grhjaxbho.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gdzxgqocf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gluvsrxiy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/goiootrki.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gnjleibij.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gfqheqiji.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gvlxfeugk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gqslvprgm.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gbhdhcgmh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gnciarwiw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gxbeubqig.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gwfbixstn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbnkncus.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gkyluthii.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gffteudpy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gylgmwhqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gwwzzdofz.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/ggvhjjdiq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gdmlawifk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gsqvqbpfu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gtxwflckq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gbpcggddi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gjnnwxwuq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxznbmfkr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmpicqjuc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gfvbexngl.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkmipvnvd.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gonoywylo.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gadfqwypk.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gqgexgcie.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gmxacluhs.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gcdvxmqqq.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gzbhryivp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gcbdzkpjh.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gempnufbl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gntcsxnud.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/ghstpdsrl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gpgdgytpv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/grgrwqmtz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gstlmrlpz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvxcntsov.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gjzfcvfni.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/genlnajyf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmaokksbn.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gkqfdkryi.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gcvxrrtun.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gcqmfrkuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gnvavgebu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gwuweqzbn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gwozfswwh.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gnauzlsyz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gqnqiucpr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghzuynqhh.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gxkdhsoov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gyeueomio.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnbxomzsl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gkftgvbqf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gfrdxoiam.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gqnftxpmc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjjvwghrw.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gycjmghpi.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gojcrrjxn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gjendrgtr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gadnjaqsu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grcdxsqhv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gypxbmnni.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gzuxnnvex.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gjollvqnh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gslasxoll.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gmivurxol.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gvjakinau.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gasumyzle.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gmdilixss.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gclhqtmln.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gniglgeip.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gmmzqdgxk.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gxebvmscb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdpfymaxc.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gozwyzwbr.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gjfaivjzw.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gwlglplnr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gomawrpon.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gbjdkbjja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/giznktzxj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/grpwuinth.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gqbhtrgrn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkexwgxab.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gzfnfjlll.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gbujgqejl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gzdgstmww.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gnaefhcnu.sHtML


<!-- 参考信息 -->