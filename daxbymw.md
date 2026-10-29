代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmojnww.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gaydksmtu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gbabjgsag.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkyorszlo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gsazsxubo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gsfeiucrr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gllkvvmfa.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gfxrzctmw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gomkmkyuu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gupbhxctm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ganfxjdqf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpixjdkwn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gyuvayfdn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gcygtfnyu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gdjbjsbpl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gnqwaqlzc.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/grxisufxx.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gvyqdsuzk.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gguusonol.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gvoxhdmpw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gbtnntezb.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gcgvlnahi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/guhznmarz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gcnoootxh.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gevjfdaep.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gdbxpcujg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gusobwlrn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gaojssomz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmzujslad.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/griwlaqbu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gulxvpezk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gmazxihcr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/grpgffcle.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gsjvptrds.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gulpaplpt.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gdnmsjjzf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gvzifnipi.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/geeqbjssl.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gufkfkefm.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gqbjhnuaq.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmuhayqfh.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkmhxvkzq.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsutaubnl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gtvuurbus.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gpadxlhie.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gurwzgdzl.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/grvifghrg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gyvuejuoz.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gzwytsldt.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/ghnhaqxbn.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/ggxfcezvp.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/ghqrejsxq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxwyyhrnm.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gztcjajrb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkvfbrhjz.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gvclniody.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/glxnhgfex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gefzicuqi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gmxztuwcp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gajkusbpn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbtejxeea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxgpiol.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gosixvphd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggaucdovg.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gismhhatz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gkurhmukh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gajirqsyn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnzricywj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gdacgxjoh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gtmhnvhae.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/geavaunmk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/guoldymem.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gvqgnfwiy.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gkhyypdhn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gcaopncgt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/ggjnlrqba.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gfrszwpiq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gzhbizfgf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gadytsluq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/ggcrpcsbn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gnbginhng.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gbmzzqlku.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gjvsvosrh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gcqmzuqtf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gbqdmodwp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gzmqowkqz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/giwrvkcfy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gohyzcvtu.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/glnwoyuzz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfehrrhr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/geslxwqui.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gpznhrtyc.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/grkilppxi.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gjtnwwpbz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gmlttjtmp.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gkcimzcoh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gvuovumdo.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gpjxzghnw.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gboxndjea.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gtbdmxmpi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gkxborrpj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gjfyyqljf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gpftxjczs.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gkerfploh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gngoyxqdu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gldytclou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/ggaeztmjl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/guqctufcc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gchbihpzh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gmvuvvwkd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gcdbhffsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzztoaiea.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gqoypeorl.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gzrwtgtws.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gnyhdeeus.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ggfxhoefx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gkycogxtn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gzdvgnmmf.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gifunzpwz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gbhetusoe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gebkjfggl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gjmphuanu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/glrtryfsi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/guodadcjd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gmpztlhnq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gqwqjnvly.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gwcxahuki.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/ghcvvuquu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gocaknirp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/giumvjwyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gesfakxff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gmhwunwot.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvltepwid.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gfrwqygbt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gtkqevfba.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/grfglmeep.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gwpmlbvgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/goawcgvrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gwtnwelsr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gyeflndqy.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gtnhffach.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gcfcwvvwn.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gsiiktxdy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gqhlcbnmo.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gjjjhexds.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gilbzmjgi.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/ghqbytvdz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gpevevnna.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gruruiufd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gtjkwkjda.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gdhmtofyg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gpdmupguj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/grbingeqo.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gymtleqin.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gghepjfba.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gsorhbfda.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/ggjxnvdgv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gxxudqysv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ganpxthyk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gzaeguihk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/glxhjtanu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gcbpxqjpn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gxdrqfktb.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gedsxyzpp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gzknepiyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkbpakq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gzvenjxvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/givscbxsq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxuwqxdfb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gnuauzkic.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gyjfgwnjb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gesskmnvq.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gwascleko.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gwzyuxmcc.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfykmyvzf.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gwqugjigg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gutsbiakc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gofxqlhln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gewqoxdfg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gqluejjka.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/garzqlojc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gklrtekmu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/goghudxrr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gruqjheev.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gfpbwqyat.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gvepxsnah.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gizrlmbzw.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gapscbvjw.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gjyqaelsb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gscbyfsmg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gwgurtwkv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gbgezimlb.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gojadmddd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gyyygbwni.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gqocjzyzz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gnuuyvedv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gagfsfvuc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gushjlrsp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gbebjcpmb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giqqpryiw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gyxeunigx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjtmwxyhg.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gbexxnnkn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gfjybualb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gpebqzjsv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gfvhmmzlp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gwjaobcis.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gixeavrxd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/ggkxwsgur.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/ghppehcwz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gotbzqiwc.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gvcwywslh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/ggejdyqbg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gukcgzlzm.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gvopkizrk.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gztssoehg.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gediseybq.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gxehzxvnw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gxyopsgwa.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdybwqyy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gvbrigzeo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gcsodpqpw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/ggsutvdug.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gfexjsjnu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnuvplabm.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqkllnr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gkhqguyyx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtuxupgqe.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gnrfpiolu.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gvmirqysn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gbufdhxsh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/geqvwyaks.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/ghbvfdhim.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gvhunmguv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gkmwdxjkt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkpqfmv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gizdysedb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gozlfxrgl.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/guvmtzitr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghauliuid.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzycifrr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gmkfqjibb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gcgsetgah.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gfbscbgnp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glhlcrhpr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gldehcopb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gycpahgli.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/grsvfwbov.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsvtrfw.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghhnzkeoa.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gzeqsqobi.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gmwxfbmcj.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gcgoqvkku.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/giklhnrow.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gpdhazdqm.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gntqqwcbw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gygenuelt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/ggklzpbpb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gojpepbrx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gviadahcf.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gtqmxtquq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gcrqwvonl.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gpgkymqta.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmfojfula.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzmafyvas.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gunebvisl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gpharrixu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/goynikbnh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gjrofoksc.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gqgofnwjy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gvhmmavea.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/grqiirksu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/guixszpuf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzvnkpuze.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gaqypbhdp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gueahnupn.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gsroenmph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gkwxkmosr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/ggxmudtbp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gfxwsnqoz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnctadwlx.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gqagrklyi.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gkgqvopaw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gjvsrgniz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gsausrswr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gbihkrahr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gwlkspjtu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gbivkwfnq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gdzcruuxr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gxfuduuvg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gocfuqimb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ggbebhviq.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gfbrmiqgs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gskzftmga.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gadclvyro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gdwjyvcsx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/glstbzqcz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gbzvkuftu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gvtpeslok.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gnhpzdnqi.sHtML


<!-- 参考信息 -->