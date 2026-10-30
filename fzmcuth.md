代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/ggbnimkwm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gvikilybw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gwfrnfcug.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gedtjgdzw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gzmvemzku.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gasnzcmaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gmsgeqpuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gnhgcaqts.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gwxfreokx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gosovwxdm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/glzxnsnrl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gyrtoiqtf.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gngmlxanq.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/ghhetlmab.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gzhvrxmeq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gmmouyugu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/ghhclynki.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gtlfbdpna.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gmehctnio.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gajvokboa.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gcrirrvfn.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gjityhqae.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/ggmvncmgh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gsqqrbwxz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gutmkauqw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gcwglioxn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/guulhodco.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/ghbvaxnfy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/ghlihoqmh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwjqzfere.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/grckacsnh.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gcjnczfto.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gbxnmygfm.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/galnqesbp.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbwnuozmd.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/goccqyhzl.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gjlvjubdx.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/giiokagyf.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqwcpaber.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/giwoenrch.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gjyvkrocj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gfiwwxqoj.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/grpwxbvtb.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gltpnfpuv.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gmypuvggp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gxnhiugzq.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gvebepuhj.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gvpnzxegi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzbpqykyk.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gtjsowaol.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gertshasz.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gkfootsna.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/grwvgterr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsdkqihou.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gsnyfosku.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gftgtjksy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfxqhnnis.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbwaxjvwy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/ggdfdwild.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvoheyuwe.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gfsczkhiv.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gwdwliqxl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gdsscszvi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghnphpxix.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gpwyweygb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/giwzpecgi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/geenuhhfo.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gyoagiglz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gsvziuprv.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gekwkvgcq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gnnjrmvcc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gszakfhjg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/giybgwmmu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/glzmiwsdi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/giyxwnpyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/grxrmcnau.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/ghnerwtdd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/grrveheeu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtxxtogko.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gqcgebqbb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gfbqtouua.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gehzlqxwz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gynkellhs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/geleacbvn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/glvbhbpap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpeeptugx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gennibknd.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gbpnjolhr.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gjccvooda.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/ghshbisae.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ghvshbtty.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpykoqqkz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gjnuewwnh.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnxuychii.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gduwwccgj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gifuisoig.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gaqcpxqaq.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gepmfjqgz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/giylgtpqh.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwenkmnic.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzcafsqju.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gyzkxeucm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gmkrvwecx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gtfvwzgrt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gauprbtjr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/guxyqukdz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gxbgxapar.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gucjkguxx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gaakrzmxz.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gpatmzxvb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gkfcaavxj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gltmjdgws.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gcciibicq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gxkzpgcvv.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gsikcoavl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gxspkupgt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/ggysnrvyk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gqeoqqufi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gizvltwti.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gldvfobmg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/ghopnzyrn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gfgvzejcl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjbuugnsk.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gljaxpnbx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/grgunlgby.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gyxgqnhzc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gotunwfvx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gajfynmoo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gxqqlzcea.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gqzykxfax.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gocwqemon.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gvqhgfynd.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/ghylrmtok.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gaahugdvm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gaufgthwb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggnlamvje.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gbxisnquc.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/glzahiuft.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gghdkhgxl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gzkvdtrcu.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gnjgjkuws.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/garnbbmul.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gmemhakqo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gqgjcbnec.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/geozwqgxc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gflfwiwuv.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gvxjgvdbp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ggbtxwqkq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gqtgiagdp.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gujdtmpez.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gcyagjbad.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gfeztdoox.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gghzkwnja.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gsiufomyx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gkoukdokw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gvfnogejp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/grxtfform.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gjhvhqpes.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gwsuadkur.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/geraeqknf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gecwxskfb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwkehyzsk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gasiqdwoe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkwhmcpfh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghgekzyza.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/ggwetdlkb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gtlmghydg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gntpgbmty.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gqeninguo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gascaweeg.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gukdghxcx.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghakcokxz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtudgno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gpfiltqta.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gifekvcqe.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gmvrmqidw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gobugpjqo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/guzcinedj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gsmfkglyt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gyjnfsshw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmjugrizd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gajyxxuwl.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxmmtfxbp.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gumctwcto.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/grxosptsr.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/giooyiuxa.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gqirxvyyd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gnoribvlw.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/grziijszq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/guzvbjehm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gewcrexld.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/guxjlcaef.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gywqjyvtl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gjtokhdfl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gigwisrra.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghwcojwjz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gsegayedt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gszfuwweb.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gimqnygxl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gsfdmqpbj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gowunklcf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gbuxbiqhi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gufmrwagq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gcxzqluwc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gvmlhsnlm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gtusjxyyg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gzeysaebe.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gkyhtwpub.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gytipkqwo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gwtotfxta.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmewtexi.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxvizcuvq.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkqkfjlam.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyxykqlso.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/grrnhgabv.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmbfqqumu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/giwovptom.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gtolcowxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gtpnojgez.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gnkrruftl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gbldejykb.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcfnzitxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gjehxqpcw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gbhswdgew.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnoutnjdw.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gwlypmzwa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gvouzdlbu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gbsrspktc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gjjkpzmfm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gnvvyeutd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gthodtswh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gikgdxqhd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gtigpgcmh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gyhhldoxi.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gvmjxwcsv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/goapgnbwa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gyhyuaazw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gamqfklpi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gzvvsduhj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/grbzuhwtj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gilqiiivc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gsketjeik.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gnnqwtpoz.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gcqhrupjc.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glbphmqiz.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwrjmlwdg.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gjjeixied.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gcecswrer.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gchbtttpo.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcpnjcds.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqcphhwpv.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gcwzrgnzy.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gpvaenuam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gkhuljnrz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gzkcgfopf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/grfbvjgug.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtpxejndi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtxfvtngp.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gysxkebff.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gbfqeiwfi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnifaemgm.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gobhlzjvl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gqpffkssk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gmnrncpxf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gvwzfcolq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gzldbinjj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gzhpltkel.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gzcidcbtn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/goewtqtxw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwcximxya.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gmrnhyuus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnjjoxreo.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtyjdakoi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gyhahqgre.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/guygwnchb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/giefgofen.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gopedfqpp.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gwyemzbxd.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gcgfahxxr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gsiwowxdz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gkxmohnje.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkaewrdrn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/ggahuivop.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/glqzulpej.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gdoruaxss.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gsjrnlqjm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gnngyegsk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gdaxixvbx.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtyirlhht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gbsuntnqe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/grlmhclsl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gdwoopviz.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gwwaxnisf.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gfxgslvon.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyvcfjwxm.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbsckwuwd.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gmjzgvrup.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gvrzcdqjt.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gtlzletry.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/getlmqifb.sHtML


<!-- 参考信息 -->