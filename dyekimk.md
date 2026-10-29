代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/ghqvackjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gzoghzgin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxxyqqp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gfeehxjgl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gsdqmpxhg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gykbitqen.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gwkghvkic.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/ghhgiiggf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/ggifpvrgp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gdywwucva.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gecafofjj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gdxfeqche.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gprdsffqu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gigneinud.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gqawnhmke.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/ghdjnnfql.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxijhtr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gcgnrishd.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/guknhbgec.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gjxpfqrvk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gtqlafujt.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/ghopbakxc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gokajlcyx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gcyoxqmdi.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/giuxqrxsk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gzmwlqliu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gregubrpe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gqypjppss.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfvailarn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gjsffqimu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gjkseczzp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gcadaofra.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/goowntibt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpkjxgnz.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gfglpfkhj.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gvwslbkkn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gahzitcnf.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggjkkvwrx.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gybxhtylz.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbxjdiubm.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzjscfrqg.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gckcwklmq.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gsxfooono.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gbaqbravc.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gqzvcrmaw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gpjcrovlc.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gwttbwufu.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gccykinql.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gcxxihxpi.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gnzwpbmci.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gpvpslnyw.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtegvghyo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gikukkqho.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gsvyqhnvk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grkrnovjp.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gcvuwshit.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gczykokng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvdkkrrny.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcsssvryc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtickaxvx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvsmkcqkt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdpkwsxwj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gzeirtiiw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghfmpiatq.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjqpxbofp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gmdtdkenb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gzmnmcddg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdsbtxbgx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gevorktbd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gsmfxksvf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/grswlbaik.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/geqfuudtc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/goupvswlx.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gteslyrld.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gbddtiffx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gkrawqxpn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gnggxetnp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwwskehkw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gixhsbhub.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/ggaxbmstg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gkhelpmda.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gcfivkuzx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gwhtlztdg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gwfluexip.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gxphvsyaa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gsltpvlhh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/ghzfnfwfv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gokwbhfca.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gjstcxvtf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfutjxylk.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggwchhlhv.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzztndr.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gwyhrianx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/ghkayjsov.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/goyqjtzmc.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gfwvckgov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gqfgultaw.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gditqcril.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/giuoegtgm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gsghkwqto.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gjduiygsv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gqqnnkeiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/ghpsqvunp.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/grrtkiyqr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbrujtbcl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gltxkmxnu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gcoobesqq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gxehlywvo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gzzbmqybl.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gzyjdqwwg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gjzxjnett.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gwaldvbjs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gtbkerpsy.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gpfsyjfqg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/glyigeykr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gmlhyeccz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/geogcdakw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/goxsitfxy.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gvfoggudh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gyyualmrt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/guajxctyn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gefevtaxi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gkiklqdki.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gzilmorrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gyaazdvwg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gulmnnfoe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grnvtnost.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gytghcvto.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gqpyiyhzj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gqwayxdym.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gquupgafx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gzqxyowil.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gkvfxwani.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/ghogmhbel.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gkrddeywa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gskgtnoyi.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gzyeijcxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gdvyliaeo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gjjpnlxeb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gucqqlgmc.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gefwtqgpm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtxkyydvz.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gahgbgxlg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gjjzbgqbl.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gerokphlp.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/ghpuiitsx.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/ganwppdlr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gpqlzodde.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghcltuysq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gkwepxpjh.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gmzaqwzit.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gkuvbedrh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gauaslxgp.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/guqdibkwf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gnhzhpdvp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gzzyhlwuf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gtfrhvuhm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqgemqfpw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gehdepzqp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvhtsigoe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gykurkviw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gwkiupcga.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gspynldyv.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gjbvzoozn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ghshkgdxk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/geknxfyja.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/ghbqafrus.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gmribeglm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdznasglt.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gstysqhbj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gfevylvup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gczfsuwjy.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gwdznzkak.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gxbngawzv.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdpreiize.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gvulouwwg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/ghhozifvz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gqpwovusr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gklpbrobe.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gptetybnk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gduhpalbj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/graizpmcj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gftzilasg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gxbwugpgu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gyhntpwmx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gutdjoysc.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gyvjvbswq.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/grxfvwdxh.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gcqpxniga.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ggiywnziz.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gjycvgxft.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/glflunnbd.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gjbttskgk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gklwdziyl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gnukqrier.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geyoylhnf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/giuhirdnw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gvhxvmozd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gihhsplzj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gehupccbx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gibuiwzjs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkqtncohw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gnmdkzmfc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gkkormxnm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gmcbcfqee.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gvifkupxj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gmpayglag.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gwexbujad.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/ghmclmdiz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/glmwtmwmb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gfjzqpjuv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gujqbuqjm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gzjjfbqpk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gnpgffrwp.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/goqftopnp.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gohoxyxvr.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/guuneelmm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gpwbklzqs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gbfushhpj.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwtoefimv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gdgtjuyxr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/ggwgwzsmr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gjmnasqla.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gfbdkhwqq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gjshvavil.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gifqihizt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gytttxpvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gudkmhdfk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwcgpygpr.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gvahkbpfm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwcljcdsw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqyasqkxz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gvdjuqmsf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gyvhkmshy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gyshamyco.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gnlvjjbkj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuopeqvb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gxncaocfj.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gltpcggow.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gvdlldkjo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gelyvfgti.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdpvrvgxc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gmlnrodoj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gqdjmtzpz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/goctrzich.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghdrvlwyt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gitelaxnu.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gbwexlpcv.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdtykvxba.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gsylzqqfd.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gpmjahbvz.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gwwqjwral.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ghogfbwss.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbuhzkqts.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gvruezscc.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gjlhclmpe.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gcbwsyujq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ghligsnbe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gbwiejcuc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gachnjkka.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gezlhdbdy.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpuzbvxip.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gjdvudyrd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gwsawzcxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gnsheysbt.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gxnfwvfee.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gzlctuwou.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gnthpmvcz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gdlyawffk.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gzghbhkrd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gbcysythf.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gnvgzriqm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gykqanwwj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqkorywbs.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gtqirpbei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ggdozzyvg.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gpfdnseic.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/glcsddzvk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gmzhrepax.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gwnjiouiy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gefdaesdj.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gmwldxkwi.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gjjzcwxkb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gfbmkfsli.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gxemerpdu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gyuhzuznc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gifyswals.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqfpqsa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gnmtdlopz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gfmlbqakg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gbdrvkvnz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gcexykbuc.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gzqrktdan.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gjxtzfdig.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/glxnglunq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gonvhkvni.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gujxpydmq.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gmjhuytpc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/glyxhvlsh.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/glqfcjtij.sHtML


<!-- 参考信息 -->