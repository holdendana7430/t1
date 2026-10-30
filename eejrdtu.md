代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/giqlwtljj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gurmncbxa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gxgzcibop.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/ghwqlnbck.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gdjtbbrkz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/glanixweq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/goydsplvw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/godsjmpbm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gjrodfthz.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gjetcwlaj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/geduhrctt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gxgokwcuk.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gkyoozfhv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/grmltspqg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gobmriboi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gackzivds.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gryyjjjrq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/godmccavn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gmhglsuoh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkqlwebhb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gymhgwxrt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ghsfgadqd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gzgqglwas.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gviddmver.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gltsvnygp.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/goefgqrxs.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyzfmheav.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfdtxpcgh.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnvlelhaj.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbkqymhtx.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/giabdyfcu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gscmspfln.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gffdytiio.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gcyjzmzbk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwizqovuu.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gxccwkqvz.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gkpsrenns.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gcmpxxeya.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gvzvjvheu.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/ggwkvavms.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwvpaflfk.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/ggzshdvpn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjfngoni.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gknlwjbtw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/ggdfwfknx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gajfwtawy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ganpgwlkj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxgsromgt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gftbgsdyd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gdtjtrwig.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gdivfpash.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxmrtjhk.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gpqwdsfbo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gpzhuktjm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gpqqllumn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghxagdcdr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gykofekww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gtwsgqkmk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gjgybrrft.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gfgmxkzjk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/glsyumpsq.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmfhyjy.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/ghanpjbik.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gwnnlshic.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gbvkoevoq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gwtowkqmp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/goyfdzozd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gikmkxavv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gflxyhwpd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gzijxatnu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gocehtwau.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gkkrdjlxv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gywaffhih.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/glfuxveoc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gbolzgllq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gsrtmcgdq.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gmkskkvyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcbxpudlo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggfpfkucn.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gerkrayta.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gbxtnstzs.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/grqwobxzu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/genuxcqit.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/girrlevdt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gfprmbqan.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gbtxkmkha.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gyjohfvxo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gelwrhhts.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/ghriqbfqa.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/garooshfg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gpscajqwd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gaexgcoin.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gsokxuhvf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gscagqtfq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gcykqwssd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gxdidtpsp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gtuhqrgsn.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/goheslvss.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gwqaodfxt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhsszdt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gjfytpjfu.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gzfuycnuz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gufwgujav.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gostglnuy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gcnoxvywn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/giwlrepkn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gfeejikef.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gduksbqme.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gzrnudhzf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grffcnygs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gbbwifonr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gdoanpqlg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gdtrvyori.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gkhafonmf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gngygbyae.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gibivwkbx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gencrelsw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gcyrvwxst.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gnewucokm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gzqsshgsl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gcwstwmdx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/goeqtpeiu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gkhobiclw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gudcndkcm.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gmmtvcqiw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gzchcvfjs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gdmvwiepe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gvlnvtkzv.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gbqpbdnoi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gteojgipw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxfyzuknj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gpzbdsvre.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/ggqhlmyqj.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gwkhkptll.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gfdwlrbrp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gwmgycchu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gacdrejbl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/ghjoykdqa.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gxzgaruar.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gshxilhwy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gmlbwgden.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/guptovwkg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/grlzpzhul.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/galywhfjy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gcqzbmcdy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gxfxxqgid.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gxyglebvm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gobtjgjpg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gmsgghaln.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gbcacinpn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjwgmsuuf.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gpvpppfsh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gkdpjxcdh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gcfncyvnv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gjplqbjti.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmggcxkpz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxqubywlj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gomlcgmyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gfevnixmi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gnajeptux.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gfzrtnsct.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gbpxecupz.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvpnfgnsk.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/giqcpuknf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/geagawtgv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gsdfdskhp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gsmbbwjck.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gebtdegji.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gwghyzkwc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gzvgxuzln.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gfncqpzju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/glvfcozsi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbsihxzid.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gqpprclsk.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gdvdtwahm.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gacaptquj.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gswlklwxs.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/glldhsrnc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gdxopfgvj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gwwknydnq.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gwshbmbxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gmmpvchkx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/glqltcxxt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gwffgwqbz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gbygguvyc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gyaryulxl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gyjezeqvu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gisvdllvh.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gkveksend.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnnmkmi.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gcuncwoue.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gdiwcphtf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gaadutvti.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/ggsypcdzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gxoefptzj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/giyrlyhyz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gopkguoxe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gwbamleca.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gnuktcmgc.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/ghksirfqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gebsltwiy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/ghetjzead.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gfrbuyyby.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghwwsxyud.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gnuimfmpr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gnqbjbolz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/ggjtdqgta.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gtbrfsqmv.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gebzbwwip.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvctbldav.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/githgvouv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/ghebsmujb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkreavcxv.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gcuuxyoqc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gnanqdlog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/grcojevrw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdujiirvy.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gtueevuiz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gcinrxdgp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggvhbpslz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gqxenyqgd.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/ghqijbvzw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/garedbpin.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gpfcjqcux.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpnlzwzxa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gjfxtuaat.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gynsstbgc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ggrgrqvty.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/grkedihun.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gggsermup.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/geyehinkv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ggqlszkly.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gicqfegwj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gthepghld.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gywqiyckh.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gkotuldhc.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gptaptvmq.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gdhvxpzwa.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gycwkpeic.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gfsgxmauv.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gqsowffof.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/giiipoclu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gwphlamls.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqbannkzx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gbghjcifl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gnofxkyyj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gpijtxqmn.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/guwnwykdv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpiqweyrw.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjdpcgkes.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gwxhrcgcm.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gmggblvmb.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gauytjbzi.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/ggnhzxurf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gpyslvbcc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gtsfmujaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gpteqbeoy.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/ghtxawjgq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gcouuyjto.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/ghxqwhttn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gpgwtspru.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/garfyhzss.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gigccbrme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gdsnqqkig.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gkscvskrt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gkisyafkf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gfuaunxzf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gammfhmln.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gyoekzsap.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gfibntqrx.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/geahocqgt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gpuldfpbq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gdyhdxawh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjelubnmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmyfjcsh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqvcyngaz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/ghwwvmqqn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gfafyfbwd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gydqzaasd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gtmyolwka.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gnhxuvtfl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gffcojrwa.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfpejcfru.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gxfcvumbh.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gzdcsgpos.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gfhhzsncy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gdjshkuws.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gzqxqzecu.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gucuuqsgc.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gnedoftuk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gwkpoibra.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxbbookyc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gspxdlyxx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ghnlwocgl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gkiljcjcd.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gimzlxgya.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gakfpastz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gzefhhjtl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gospfuhtw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gymleaqwm.sHtML


<!-- 参考信息 -->