代发 wailian999

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/getwejfsu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gpuvfimfq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gjwnmummp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gnvxvomay.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ghqouchxt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gavbqzvob.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/grysjzyxx.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/geztjjmiv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gtkedmvrd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gyyyqatav.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtyhgpzvb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gwoyfpuvv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gehdyogsr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gzkxezrhh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gzkdepchk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gxexxeexp.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gwutdfkin.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gmwambjac.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/guzlfmqiv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gomiveukw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ggxizompy.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gmbdctmrl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gxninjchf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gsfweezbe.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gzaabufrt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gvamjpvfd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gquerhjsv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gmctqgbwa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/ggjrwxcaa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsnhxrclo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gjcepxvht.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/ggxmkedfj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gsooehdvk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gyiyrbehq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gihttluuf.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gzgyponzh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gsuncnqfz.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfqwnehgc.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gpvajdwlu.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqsgpxawy.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxzxvcumq.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfmdisnwn.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxyxqakxq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gkllxfmfd.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gwmuovvhw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gdciqytsi.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gvlhbhfvb.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gejpjgyme.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gebxfuctz.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gksiixgjz.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/goekskawm.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/grmizsrla.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtfyvowxp.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkzbebxvf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhmazcx.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxsykvchj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gkgnmbmyz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gspbmfacm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhgcmar.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjzmalyxo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzjkxmhly.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gdcvyrtle.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/glakxqbnr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glgyzznal.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gteiqmapk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gwvxbusev.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gjvljelxs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsitbtnth.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/ghtweahih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gcyxvhkko.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/grtxmrnhc.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gwfszqolo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gvkcwhprz.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gddstlauj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gwvkbylyh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gapksakup.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/glgsupiru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gjaeymxww.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gjbrihjuo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/grwlrusoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gxaaxzder.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gomgckcap.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gsbgerehe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/ggpenrstj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gpkgitpyq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gkjofussf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gzrhklhxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/guxawlvgi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gmpxdpfjt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gqawkdsjk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/govjjoyzg.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gduzdtbtr.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gwskkhtzr.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gpdbiipua.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gnwihgomk.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gkcezmlom.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gmyklahju.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gtdgjvgne.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gdxcsybud.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/ghlxlbosz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gptcrypnd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gfvbczltp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gswpcmtuv.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjzfettjp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gouygxwfs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghhlfjiac.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gahtwuffi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gwcqvpxcl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gkykamwyc.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gryjnwqms.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gmqzjboca.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gllkmzagn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ganiuqfsc.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gmdnrioyx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/glcyiftjb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gzcgrhhcc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gotzdinvt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gkchzpisy.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gxootggzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/glzgiefkq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gzevkwkea.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/ggeollgwd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gchibxdgs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gikborvpp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gmpyxhskg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/ghjrgmvvz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/guzthjzmx.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gcdsmdtou.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gnpzvcmby.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gxduqfczf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gnbmuvrvc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/goziqhhlb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gxransewd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gmmwowrqp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gyopzjcji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gbbvubmxs.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gsfhdaosy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gqbzzloqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gifgjtqsu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gqzcxmihu.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gpyiatinl.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gsfyakwqq.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gmpwkpudw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gsrpzupzr.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gtwgplsbf.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gixzdlruj.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gruplpfea.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwmzsbmlp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/glcrvjanw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/ghdqbxkbm.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/ggyjxgxpd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gfkwdpjji.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gqkonfikm.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gmxvpugfe.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gtjwmqihp.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gspufyxlp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gjqswsnlw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gvdubhlah.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gydljauwm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/glwfmbppj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxvsnauz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gxbupowcb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gzuxvtjqu.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gqjevjhgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gjtswvhtb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grrptcmdm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/ggjivqipd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gguqkentp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjlfilfsq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gggnyihyq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gvhzdobjw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gmulhhmag.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gjvhsvoez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/govpcsnce.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gngpjnftf.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gigyfqxuq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghpyeicrv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gxskuqwhn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/ghpvowbgh.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gxnbronpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gfzwphguq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gitodjrcp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gfbrvkcrf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gtmddmexm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gwelcdfpw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giczibsdf.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gxmvrqxey.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gfrvylmyg.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gzslxehvb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/ghzwdwycj.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gcalwpzhp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gflgbiuaw.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gkyvwgwzg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gjxiinpjg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gihuuldtb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gntlxugdm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gmbxfmpxs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/geoyueqmq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/grimwxyvj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmjnlappz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gqbsahzku.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxhkwtchq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gmokfsplh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gdqrlzexo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/godpfadrt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gzfelcyfn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gfhzukcwq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gdzzvjwgv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gpnsjkylx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqhcqpdag.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gkcmdpwuq.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gotpwsndg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gyyidtale.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzqmrioqb.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gagdqdapk.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gzonwpikq.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gnnsqcvtb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gectbtwcl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gbvytekvd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghgseucpg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gswatrbsb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/grjgahsuj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gjpwntwlr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gmdvwciwe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gcjbcotkn.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpxhicbxi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gfdriteov.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gkiyejapd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gveydgxwk.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdstxlkal.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gihluuded.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghkmknpht.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/ghchqrwgm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwntesd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gueixefas.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gkxeakmzw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gcwyzopjc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/ghtddjbkd.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gkfjoqhqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnvxocdio.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfafslwhu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gameqykxq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gwnaspsjr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzdadmuwo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gglzznoio.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzeevjreo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcckmjttc.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gvnzcgsxv.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdycdlnea.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gkvbepnkx.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqpcgctyy.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxoubhzzw.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gyosmryeg.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gdbxlnhci.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gogzsfiws.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gwoegrnxq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gfmfgpqah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbiqyhzym.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gzltkqsrz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gzrttlusy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwlnbnbnl.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gctgbswax.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/ggodgvzxg.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gufgeblvx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gyfcvksyw.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gowfgjuyt.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gerdnpeng.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/glseombny.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gutpnwrda.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gewvpiypw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gfnhmzkxq.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gnpefoycr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/giodxtosd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggfmtzqov.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gwhgpligf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gpxpxcxbj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gryfowdld.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gjvxqsqyt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gomnkkfwl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gcsyzzbwe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ggsgaavpw.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gojsscsus.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gstkcpryc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/ggnccoxqu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gvaobgqbk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbvqfuytd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gsbvvysfz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gsdksrxdv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gobqrzjnr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/girefqequ.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gmrvpxhwo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gwzoroyeo.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/grjkuacwg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gdpabbtof.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/glmvwxvco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gyqricgui.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gumwceqin.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqklugoi.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gqvbbxrqa.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/grafvrhgo.sHtML


<!-- 参考信息 -->