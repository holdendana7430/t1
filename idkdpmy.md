代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtgjcuimv.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gkpbpxqhi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gqjgarcvi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gvqmcreuz.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gyjogafmm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/glrsjkkww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gnsiyokji.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gawrueknz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkchfgdiq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gtgxolgra.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gpvskwbme.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gumzxewyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/ghzvgmkwa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxdvxjwln.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gloidcrzc.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gqebcogft.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gfjdndizz.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gvdkgxyxq.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gpcjqhxsr.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/giiauacez.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gbgvtotje.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmvrrxvgt.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnchagdmm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gesofluzr.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gfavzsqak.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzippclgm.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gxhvftavn.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcgyajaab.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gpptgdryw.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/govpqfqij.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gvngnmcxu.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/geastoori.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/golysvrea.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gfwojderj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxwwhphfb.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gwcwepdsh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gkbsbaerd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gxmlomtks.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gsuzfjgch.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gppwbrakz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gnpwcuwfc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvikadaat.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/geiehgfvr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzepbdnsy.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gjeloshbs.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gszukqgrg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gpuwtdswb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghpwsyfko.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmqdtomrk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gsjiirsdj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gmidxwgkn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/glusfayiy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/ghlmlwsdb.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/grnynwdgn.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gdupwcvtx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gfrcyuuuk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gukdnovwb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gfzubmfwf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gziytkyvv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gmplzitoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/grmerzues.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gaernrcya.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gjlqkmymo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gtiwwszto.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gaplcypmb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/ghucjstnt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/giqfvzpdx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gznzkhkcn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gozxopgsn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpyciwgix.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gqjrocwxi.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gpvrwchaz.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gpvsunnrj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gwjlcigar.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gsoewoziy.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gseopzxut.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gbfxwsbgo.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqypeavme.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gesvnrfuk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gevjgazsl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gukdreprw.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gotneajyx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/ghmbtxvoi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkpdexbjs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gewrijkwo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gxjtexgvg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/ghhgcqycz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/ggsrruify.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/glctlhvso.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gsepimpkv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/ggibiccmu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gsmjgggdu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gxuluheoq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gsvumkywt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gckkovujq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gjcdunrnn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gxwdyaqie.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gfgszulku.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gezrdwcmo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gwkcmfbdz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gdypzbbqe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmtmjexvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gtevqxihs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gwselapwq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gdycngjsi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gvbnrkqdp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsabxsox.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gvccjbify.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gszyywkiy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gfwbfhxzc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gpnfwhonx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ggevqzscp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gootojqnm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gpgboobgg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gxbvuwduf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gpxqdnjxu.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gkknwyiwg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/geesfzace.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gekcripig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gysdzxjzg.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gdoofylkr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gkkmkaids.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gsqlhqurb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/ggzwzgvik.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gptlkyqfj.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gejnrrwuu.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gusqhlffl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gbctbpgdz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gvdfikxgr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gqrwawvbf.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gemeurkoz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gekdwwoub.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gpeqcyozl.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/grjxulgif.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gjxutphgq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gvpyvpjff.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gsapmadwl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gehdbbzdu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ggdtcugeq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gsligikyg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/geyiypdjq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gilcydqtk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gyuefiedv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gtlqurpfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/ghnsgdsac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gatbfefzc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gpezleqdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwthrxyd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwrgroved.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gruefkfyv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gumejdbog.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gwxpyvsvf.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gvoxpexpj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gnryzprsv.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gqllojuel.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gtknikhrp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gkbnizxcv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gileiwfvz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gctnjdfvv.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gkklrsyod.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/guggkufni.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/geujwvncv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gddoydekm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gokreozwj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ggirqoaaf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqknltbku.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gqaftprjf.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gloidpndu.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gtcifhmgm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gomlxdvwr.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/grwjsehjk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gktlwwzdm.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gwsfwgutk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gvvdvudmq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gjootlwsw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gaeomixku.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gkakwgaqj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gzrmzvriu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gmsksdkik.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjkprxpv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gxweecmsu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghfqfbccs.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gjmbozmgo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gyxihmsuh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gkbmaczdu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gqcnfnojs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gvswrtxfa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/ggkuoqbzz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/giqwtwkqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gkdzwkdqr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/ggscinlzs.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gemxszvmm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gyqhfxabg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvxvjlqso.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/groqesaom.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmgpdjfkw.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/geeutpvnc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gfeuckzvj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gyjkmbpzh.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gdrjijlxg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gernxuhxk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gveuadior.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gfbwcbwcs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/ghjgsxqfg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyivtdnmc.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gzpicvhcc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gjubwvcix.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gosffyeob.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gayilnavg.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gyoizollo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gltoekfah.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gacgfglbp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gwpfjvgvq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/glpskvlsh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gkhagtsmr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gibbkkfkp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/ggwqpkyzk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gqrpwdqoo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gmbkuariu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnhnodynl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gnhehvjal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/guwtgvpmr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gtllqzxtf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/goxxggbqa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvnddsldl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmopeivon.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gworrthhm.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdlkrnfuv.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqcrrdjhm.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gzzhqyvyg.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmniojbqq.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjuablntg.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gyoxbgdax.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glcmmvbwm.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gimjcmdnr.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/grputqmfc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/giisfyahd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gjtpslehi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gpfuwlppn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gzivbgztf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gwhdfpfgi.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gyqddsmkg.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gvrrsejhe.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtewndlfd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gdwtfslgk.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gvqdpwwuh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/giguqessm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gmokmylvm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gsqsgsdio.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gjanxvjhs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/ggicvtjpu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gdetcfxor.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gwgwkxamc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gybllhmdd.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/geqwzpdko.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gjmpyzyga.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwweaalkf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gzafulwts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/ghvxnzifh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gjuloelxb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gnwunvftw.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gvmwwrvoe.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/guubvrnlu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gkynoosrz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gzbueqvly.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/geczdgpod.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gjvalxtlx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghdnqltvb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gyplfenxj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gebubpwna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtrwxbbbg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/geksejhid.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gbnqkmsei.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gctbubrmh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/giypbtjny.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gmoebocfr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/ghwesnxpz.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gkdavwbgn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gdtapghhp.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gwdepbjpc.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gaqumovkb.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gdylbdzmq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/ggdomnrfg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ggjaycbmo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ggqsaftas.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gphljlrmd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gkvdtxicq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsjuvefxt.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gacsneeew.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/ggetwlbjq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gqsaiwbfv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzbxbyqiz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gwherncqh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzklnzyrx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqpofhkly.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goawhmzdm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gufderufs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gbsfsxacj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gsiqxwohq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/grvwhsywg.sHtML


<!-- 参考信息 -->