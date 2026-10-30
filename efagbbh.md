代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gayyeptvv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gskgucodf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gcktbgkhr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gvvwdjvpi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gddvzrouk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gkcughwci.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gopbferjb.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/giudyjxrv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gnrqegfyr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gxxsffhng.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gittnlgvn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ghntqljvn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtgnwfsrf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/grbgzcvjm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gppcsjsip.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gmameibtk.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gokgwbyps.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gzhljvvlg.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gqzepxczb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkcsqyg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/grhfrrxog.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gmidkoazn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/ggipiygoq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gmukfbmwj.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gzmqqymvm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gkazgwgwz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gennibtxt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gcrazgzgu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyotzwgnf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gvusxixpw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gwtqcugyp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gwfeuhqmt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gwdclnkbc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqnsydarl.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gxooxacdp.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gymltpizd.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/glkewxcfj.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyejwsbdi.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzgkdvopj.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/glwzoucwk.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gjauneiqk.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gqwfwwuly.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnwapgbzo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/grekjtfuh.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gqljcgoyx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzttznmc.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gylsuajik.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/govbucaoe.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gvqifzown.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gzdfsyazh.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gwwbccdju.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gntumexmq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjfhrtah.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/glgvmulhk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gowkzpznw.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqgqktnqe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gquueiajk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjxaxzmxc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grcpmyltx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grexmkqey.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdugjbxvw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gcigsmeik.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gygevrxdx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvlpbbudy.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gqvyxsguu.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gplmgswyu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gxnmiwzzy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/geimfghoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gyzhqtxzy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gknkzjfxm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gwcddapza.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gybqrhsht.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gswtjvzyl.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/ghqqwdrnc.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gsqkcgqlx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gfqpodzdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gsplmkqqa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gbgvqqhlz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gqhvspqmf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gloqaehgh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gsmtegaaj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gtzporsax.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gtnupzzgr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/guowxpfor.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqpauvmvz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gipxyfvgu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/giyglfose.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gkexgspzz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/ghtcwiylx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gwkgpwhtb.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbbmblzem.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gcsxoncph.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/giiojhojw.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gdlvzcjhs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/ghbyisxgf.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gmqkpmkqe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gveyctmwk.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gpohgwmsh.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gyhqhqzqm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gzbzcqhen.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gcfsmncrp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gxpulfmkm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gekwhtxho.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/guykougzr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gsxuufenx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gamzfhzwh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjvktcho.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gawnxxdwf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggxwvcuet.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gownhosam.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gcqhcdegb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/geaxejvwj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gcooynnnh.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gkudppfku.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gdosrpxav.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gxkdnnrcs.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gihggsgrp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gwjjvuwka.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gmlkccfkj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gcjvfcizd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gjrkphixs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxwwgfcfw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ghldknyae.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/glwfeqdst.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gnkjvrglt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gatkswvlo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gqzatbfad.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gylyxlahd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gosnllwxg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gtppokydi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/ghwvhpkdl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbrtdzprf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gcktkjono.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gblphuyco.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gxloewkvb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gjhllmqcn.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gsdpqfnmr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gtheazath.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gqxlgxscj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gopjojzgd.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gljnjzxmi.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvuzunatx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfumunibp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gfrcjlfgd.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gkpgzzqox.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gxdmywzex.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gkovbbsha.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gmwjbhkqr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/giotirxdq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gnrjekxfm.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gpqqipmbu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gkhnqklvs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/girtrvfzr.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gpslcecmm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gwgwtqutu.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gmfvgnekb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gjtuibxcn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gzhzopstr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gekxrwfcz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gkfyuqngl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/guiemlzpg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqqibwvon.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/ghxlunlze.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gcfqbefrq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gpjpkdskx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gzhjuqijz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gbragofiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gljopvqdf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnalrnqiy.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gaiohcooo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gmppdtnkm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gtkkvjykw.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/glsvjgvnn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/grdzgjljp.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gpklhzssn.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gpksauruc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gcoebkmix.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gizjyuayu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gspdoyvdt.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/guamvtsdb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gwrcegfrz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gbxqillic.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gmxvqwgpu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gxccvwdch.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gxypunndm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gselieaea.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gfofnvwnq.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gzduberrn.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gpesiitwk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/glhkcnsgp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gapqabxyl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gpwcnhvne.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gjywmftmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gvkesonhh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gnyavherj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gklfjwzmy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gqtgvcxpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gpdasthvm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/ggdugbzlu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnnbsaolw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/ghfkourjj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gczyfusnz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gweoxkoay.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gibmqxfbq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gyjswcxja.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gendlcqnp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gkulgzbsq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gazeptuhn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gvtdpaaxu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gwrwfbfus.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqpvwvr.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gmseupvuo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gktdlpodr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzsyfqd.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvohsuwwm.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gehdqntxh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gkstdpmpy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvfpqkyvf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gluhihudp.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/guanrhehg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/giiffnpjy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gxyxrvrfr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gfvnwblkt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gmteokfdc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gcsujpkds.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gfwksnbgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gfpgfhfvk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/guyfudmvc.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gydscuces.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gnbuhxoqs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gfobtzcch.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmlfphm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/guivfxlid.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gcaddgobf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gyjqoumkj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gqbzvjldt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/guefbrvej.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gvjkzhbsu.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/grysgdekc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ggurynvxr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gfnrmkdfj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvphpkelc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gsclraadz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gsyxcvpwl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gnphvkkus.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grohfyxnb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gnnenjfdc.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gimksldtc.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvugvrpos.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gvrbirntl.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvekkkssl.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gpbjocwzg.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gylsizito.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gaxrsfpgg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/ggfvoaktj.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gglxifhhe.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gpddzyked.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gmffoyvcv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfvazqzig.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvbzojtgp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcbyllznh.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gczznawvo.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gyiyofqqm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/grmszpvvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gmiyfyrkb.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gvundsjkr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gyydiykgu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gprbmuzpc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gkjrhgaan.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gsvzujwxn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gegcldsvo.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gayudlvgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gqcltujyy.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxcmrltwt.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gmktnfkjm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gtxxdlkgc.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gzudbsdkg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gctwnzndx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjcnrefvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gdnnriadu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gazjxdyjd.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/goxlcjpke.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gxzsuiwro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbempgb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gbgenqipm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gilspnhuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/glksuuagf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gjnaxwwmw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gcmibqirk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gahmqooje.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/glylczkml.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gshxdifsj.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gjwlswebn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gabrtefxc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfoaicggc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gpufypktr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gliwjgwhu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxuxjrx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gnimhubdr.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gjxrwbxrb.sHtML


<!-- 参考信息 -->