代发 wailian999

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gpbnddeyv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gvyvzxbaf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gydduqwhm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gxxvumvra.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gukfhfsvb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmjixccuo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gnycudhqp.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gabozrxwf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/groydzpjl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gyedqbkrp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gixdzpoxo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gczmxkpjn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gxnpodkja.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gcaxyzley.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/ghxueyjls.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gormwkzef.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gzohgifyd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gauclvqjp.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/glajfmkjy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gqxmgyyui.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ghuvqntmc.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gzbjcmvaf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gtfwoesgl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gbfdandvn.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gmqehstof.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gqorhgxdj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gzovcejok.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gjiwnsvga.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gobueerer.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqlukjuga.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfzsqccnm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/ghijnqhit.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/grfmtueam.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/guuciigaq.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gzcomyxxb.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gpdoihvfz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/ghcjtfuwp.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ggabahfwm.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gqufgjztp.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glozbjbey.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gaurnkzcj.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcugybpaa.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gnrglhxbu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gqibkktnc.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gsrhqxlna.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gwboyqdwy.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gzqpjfinb.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gifpqhysu.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gdqpqemno.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gpvghajuj.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/guyzsnfam.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gtslovcdy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggdmuolpq.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/ginvhlmgy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guahmxpan.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gbpfqijra.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gfkwmvvwo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gadletxcr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gmrhsjchr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gibpgathu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/glymttpgy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnahzluwh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gmlcbpasp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gtwloijnr.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gkjkzgfhp.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gmdoaemwu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gvsntcciy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwhhvihod.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gmkvmylwv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gcaukpkeb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gzshdqdms.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/grlgojmis.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/guvrdwxty.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gmqiugrjc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gjeymozhu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/ggykgmpmh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gxmvikiru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gdazfrhpc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gmvtdksbc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gyjujfxdc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gcotyqtgx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gpyrimrfa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gvkpeotjz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gndjoakcf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gbdnnhoou.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gzfydyxep.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/girfvzaci.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gyhwfbrio.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gilqdyhhj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsobenpxk.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gygevajpi.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gfbcawfqe.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtruhzouo.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/ghndyxtlr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gzaerbxdn.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/giwtlroeo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gznfjtlpo.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gakqrqhqc.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gwongswcv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gltjviqfv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gjrqdoxzb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gqelapdyi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gajxpqkss.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkasdubzw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/guugfbjtw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghwpeikza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gmdpetaag.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gsycveqiy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gykylmtxo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gnsytxsjd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gnnwrrdtt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/ghqkjfddr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gqkdyiiph.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gubhsfnwd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/ghqojmqpu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gztgupwxm.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gxtqblrjd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gfyxidjis.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gblresjwh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/glpfgphro.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gjttqeyoi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/glikwgrap.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ggjpanset.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/glalmhilk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gayvxvxdo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gqhjfhxic.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/grjlljwpa.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/giteesvjq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gudqtbfjo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gfpfjgvqi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ganbqdwau.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gspabgqxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gmnuzchws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gyhfgqmah.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcckdtzom.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gtkcjfbqp.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gvyfjwpem.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/grsjgphqw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gsyvxyxcd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/ghpgxvahs.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/geecswkre.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ggbahizii.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gsgxjcxzf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gyiqekmro.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gjibhztil.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gpvbqzlzi.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gbthmfynf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gcnkzmdua.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gnralplec.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/grboqgcyx.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gzpowitkt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gscymdsqj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gvsdklgeg.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/ghuzyuhjx.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/ggimopbeq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gtlisdrck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/glomookyl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gmsjvabot.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gkeetqzwq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gihlpxgfe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gmoxiuiuh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gwilcynpt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gaiurlasp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gjjalmywc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gplfkuvjy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ggaalxhuc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gelcctqup.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcngfnkqi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/glkjjxehr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gegsdcsot.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gjcieozrn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gzhiamovq.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/genqdytkv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gyivehvxh.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/guajbshmk.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/goywzyllm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gaesblgse.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gluekfjnz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gkpithhrf.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/grqxxnuzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gtgxqrino.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gjpnobpru.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gunxgidmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gkbbbdakn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gjinepmii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtxoqkrxp.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gyunuikhu.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/grspqiqfr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gnaufrpps.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gmxxnhxdm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gjzzzdzsf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gdwhnjhsv.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gbhogcaqz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gashdaklz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gsmdcxhtm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gjdcguksf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjqrkqdqm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gtvrgapda.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/geclcmcum.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gichogvvo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/guhdnmyyz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guulsfclg.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gofrzpgyu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/glcqudibl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/ghladkkcj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gwkpqvmrt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gjicfnkio.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gzkekindd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/goajtcisx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gwfqoiyty.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/girkqcqpw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gmobeodem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gkfenosds.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gqlpjwlyi.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gzoadpcan.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gzonvciqu.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/grvcxsaco.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/grdmkvqop.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gzgfvzfyu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxuoaxgkh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gskuyebnb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggtdtxdtb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/ggmeljtqp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gnwgkzskt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtirrzmsq.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvomjuvvk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gtgxbrpme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gbqugasyo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gjepsvlfs.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/guicmqrzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gxanffsvt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtnvhqnwr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gbahrwsul.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gleuwwgrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gizgjzaly.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gcermuxwh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gsamutwwn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gktjsfqnd.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gfrrlygpb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjyzbmftf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ghhvashpl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gdxvplrsv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gpflydxwb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gzqmylmuh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gctfyipmd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gzdzihokd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnvinzsjj.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/guddfqtlf.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gynrrhcvc.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gttwyvtsq.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gajawgftu.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gzntmfsvu.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gceozvmib.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gwscmzhns.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gjjfdrvix.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gmmwnafhn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gqsraaegh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gvjkdcayx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gprxfqhod.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gnmuuwhju.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmhypwwvp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpufrpwub.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gcgxknpeb.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gyuveeumx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtmvammhp.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gbzfvnnon.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gvdbwzsxr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/glavauljj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/grmrcgonh.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/giamxihtw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gffowfejp.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gjzqoxsxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gndmsqruc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghcnkqmsh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gkwxekwxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/glniahhul.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/glcmuyjlx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gufokqowk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gcuddldmg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ghivuwvml.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqbyehvqd.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gvpqqskjf.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gntdluqsq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ggkpbelhh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gsrpsrmcq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxpffssqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gigpouhdv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gviitfdky.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gfeqljooh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gjpncfyys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gqkmjvsrv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ghkrgxuws.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gdedarywt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/golybyrab.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gibemrrbt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gdbgcztjh.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gdojhugay.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/grgdwikpq.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gprpcrfzt.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gdhvvxtxs.sHtML


<!-- 参考信息 -->