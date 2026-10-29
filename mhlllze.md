代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gzhcnlmgs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gnrzjgzpv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gblegwgfv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gsmyuysoi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gtqjwnscz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gzghrpscr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gzltpaomo.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gzpfolbyo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gysijnvyq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gvjhbucrn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gktwqoeiw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gkvadxhjh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjhngnwhc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gbiawcllq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gmgcttlsw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/grpuonmbn.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/ghjnhkmvv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/ghsmylnif.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gcjioapgv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gpklsalai.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gmugjmhyw.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gdtwzjwfg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gayaptsdr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gtcoigzos.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gvtyxlwvu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/geslevafe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gssanffeo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/ggnmczwss.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gxdrwrsrg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gwopcuxaf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ggvryqbxw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyfvutmyj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gwqlmyglm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gtgiauczi.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gmxklkupy.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gfgnjjjds.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/glvoknlad.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/glxcidddq.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gpfclklvi.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gztcpgpds.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggovporue.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gnrfieznq.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjwomvfsu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gmealwkui.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gfxnqxadz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gyfaqkast.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/givybgfrr.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gpemzgdkh.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gllzuacvt.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gueqbtgeq.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gfvkcckqv.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gucxohgbp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpgsyhmen.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gdykiykaf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfkwulbgu.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ggvcqixea.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gkqjopymg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnoeoguwo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcjyokzq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/giekmbmch.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvmrngag.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gzrxwgcte.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/ghuchbypv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghewgzlda.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gyjjebosz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ghhotlzqy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gomdjveln.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfecppclf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gediartar.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gmembcxti.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gcmgoghzr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gvpalkimv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gsgeybifc.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gqrnermmq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gaibnuvtj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gvdeqzeuh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gszggppiu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gpooxdqfb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gwsnxntbn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/garypfxcq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gmvbksufw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/ghpmcbztw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gvqgmhyna.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gfqnwxloj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gqubqdqkf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gfyqudskd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gfthczgjz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gowqvdbtq.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gdyuaqqtj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gylynfgcb.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gqbelhozh.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gwaniihko.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqbpogpfs.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gmyvhwrhn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gvuvjqcmt.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gkwjrcapz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gmhgdtuct.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gzebwrrhp.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gjrdayhtn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gpajhvrjv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gqlgifvnm.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gmcfrjwfw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gqbcecfhb.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghtpzzpij.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxwbwtnkl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gbblrgfmi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ghzifyhwb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gphiiuezq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpwnitjwn.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gjmoljvdj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/ggamjbmzp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gnnxyntst.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ggdxogfze.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gkbptwpdf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkrchlkac.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gbpnxvdrl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gofzotyfu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gsbkzadgr.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gbthoxgwg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/goqwcznts.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gvfhbgytz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gxxxuypcm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gbyokhbbw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gppesxwdd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gkagnnbjm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gekkpbixf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gtxolwmhm.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gnejjwloi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gunjlxpxo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ggtzbotnu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gequuccft.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gbsswrikf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gogmcrlfy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gqhczxgcw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gbtkdkbug.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gvlytpzut.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/glhygtzit.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gdodwwcno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gybgbpmcv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gqluqiflp.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gtkyuqelp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfzetagej.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gsoqlvdth.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/geebioywh.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/ghadrbugs.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gwqhsxexn.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gtxhhqjtm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/grqtalsey.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gnhbdvxmx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gjnmevfml.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gfoggcwbk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gneldehkp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gpkpjlgfx.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gvtvgxwki.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gqzwikrob.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gpykeqmii.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/grucvhcae.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gfmcvnoud.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gboykxdkx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gtxpulzjm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gvywbkrft.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gadclevsn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gendifgnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gzxumcxpk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gsdzeylko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gswhxyjcc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gchgisykj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gdqanmmmu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqckyrnxg.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gsthcrlpr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gfmkwfyji.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gkuueofzr.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gzkzqlxyi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gjgldbeqf.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gcapgjeaz.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpunrmgsa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghebdtyus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/glrybmixx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gcgpihnlj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gecejzmdp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/ggsjzngyo.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gcupjechq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gjvazttym.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gsmrkconb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gklzxbmya.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghlddqcmv.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gmsxkwivh.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gtufvlwty.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gdyjnypgk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gfrlkezlk.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/giwwynaek.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gmomnfirr.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/grrrunpnb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/ghaiculvc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gcgjhrqfk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/glsdzaqjv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gmxfbamtn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gtnaiqmfg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/grrweghqd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grpsiuqbi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gcfdmofae.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpwelcruo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/giptczjpq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gyuppfjnt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/guvcvdsti.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gufwxttzi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gahbzofyo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gybwgmnrj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gmhrzodxz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gwztqykoq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/geebavbci.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gmcibdxyy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/ghivtpttu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/goxzqmpli.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbtyrcrqi.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grxrylhbv.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/ggyacastb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkeaenrqz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gfgxxpsgp.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gjtpfcfqd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gmvfrcmio.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gflaeqepi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gtbnnkfoh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gdebjmwkc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmhixgald.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpfwewyve.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gzajsmzop.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/giokohanc.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gszpkvkcv.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gmfnrhsrd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/grygsvnvc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gteyzlmcg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/godorqszs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpwzazrzx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gghykjlxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmttwxza.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gnruucacv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/geiexrqnr.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gwnefaisf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcwgqkgbo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gmgzxccyt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gveydbads.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gnsvgimki.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gqvaufuks.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grhhgamzo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqnnoizsw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gukgguiiv.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmgzfawwc.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gohfkoukr.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gegqgqdbc.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/guagsnrcc.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gpvaiwoyq.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gcasclrhm.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gppamfilj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gxkjaiofg.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gubocxwfn.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gcwalklxy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ggndbuibf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdbibwqcp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gpojcdimm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gqmefblzc.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gypyzoyuk.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gyjkxpqne.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/ggcfpdolx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gwurwaqra.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gmjofpdsm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gitfwgkbr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/ghdklvrul.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gmytjjmgs.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gxlifdphk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gsdgnaakr.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gstrylfvg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gwdkrnzwj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gtjifdgxa.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gnfnrhxhh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gimshbjno.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjehphipj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gngfrqtnp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gamnhodfl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gomvpzyfm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/glyfxxwby.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gfpqzssoz.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/grcfhlndc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gvzsndhoj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcqqacv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxnsunebj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gzeupwsvf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grtedwrjf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gkheyuhvy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/ghdohvtoo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gqjxigbnc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/ggwutejod.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gypzmlpgk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gkwtnfkjj.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/glkorrent.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/giyylfoxl.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gyfjhjajz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gnakvhhgs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfnthnsgz.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gzdmxatuj.sHtML


<!-- 参考信息 -->