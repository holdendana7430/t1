代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gduwzkoej.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/grdekgtoz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gjznrbfoi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/greqemuvf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gattlgbiv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gjlqqnuwd.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gepgrkfjc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gonlkmwil.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxgxpvbn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gjxckgvcy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/glcyoafxx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gwlaoeiry.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gedpyibjo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/guwebgtsl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/grtsayyot.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gnqobghbc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gtnuespuu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gmatuvvpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/guaobwamg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gokjhpukf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/guzhqfzqz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gdzjclhln.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gwiimicck.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/ghdzddaoo.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gkukrgvco.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gdrwlfpaz.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gsgbpkeag.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/ghvrqdayo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gchklbgxp.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gyftdkekz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/godjmaevf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/ggnxvwhwz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gfvmegbma.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gznvbydbx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gagubnmhr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gozjxidva.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gmhakbagr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gdmnbuumq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvqtfzvjx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gwjwotnpq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gugygilmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/glpkfpupy.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gfoyvumma.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/goeleriqm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gwdpjmtqy.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/guerdostn.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/goalltcqw.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbyetmzpp.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gaooyxjqz.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggbdzctxq.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggjiqwdez.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/giflecijx.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gbfdnpgst.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gchvfmyov.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gxqzaagay.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbswogqkf.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gcwbvoqkp.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gphjszaoh.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gypgaxuxv.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/ghrchdipb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gevgleakz.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gflkxpgmh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzryalaqk.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gyvjbkmhw.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gwqhuephx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gcwujpbef.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghjzyvsaz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvgwykzrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gygpcoayl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/grjftvvna.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/glvfyqxzv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghqjkddeq.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/guuaguyin.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gaxdembrq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gxvqojjos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvduvjkud.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzyfhkljm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gbpkdbmip.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gsxxqjavj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gkplokhjv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkwqhoyd.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gejstbnvm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gtcekbppq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gyrqvicwy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gkjzlyank.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glbokcgis.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpoebbvji.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/glxhcbseo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gfejjcimm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gpeumgdow.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gleujkvjm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gryavsstx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gifrdvsox.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gnutdychs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gyudasikm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gnnnkhifv.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gjikjpvgr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gqikrbzeu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gqgzsuhot.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/grkqmdgpe.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gqbainizc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gdjxuiyst.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gjprncxjq.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/glsqdgleo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ggsuuvbcv.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gajsbixhp.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gmywtqkvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gjhockmwl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gfmnzrlrk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gcvhadfpt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gskyjvcsj.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gyifbchoq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjmfoddex.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggmfbioms.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/ghatlzbgt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gpqmyzugj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gefmunrsq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gnzawklwe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/garqynkje.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gevvcrbcl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gmoxtcmns.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gzbwyqnnm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gllwzdrcs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/guixawiid.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gisdxxjaq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gklxkqyfu.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/glkrimisk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gptecghgu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gyyvwrqoz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gaglbwzwm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gomkdzmvo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/ginxypcvc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gjhclgtdt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gwtnnzdin.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/glskyurho.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/ghmiksgit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpwywrtet.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gnudmegli.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/godvqlisa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gcddkijrx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gnwyaoewf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gqdzpbggf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gfgbmnzuq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gngprfgno.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gzkrabgja.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/grygfriuf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gdymbpscr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gcgdzcmsb.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gngapmiqi.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/grfnkiixx.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gqwafqzpb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gmhpawmgj.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggixjpvtw.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gvmpzcnxf.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gpyumbxko.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gxwhnpvms.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/grwzubonj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gafycecuv.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gozohlvjr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gthiksqyf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gsxzjisrc.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gfcnorizw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gxgapyuvf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gqhokkeqg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gxakurzli.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ggbhquyad.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtrdnfzfs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gfrhpedaz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gncdbqkvz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gtupimofj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gtdamzlfn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/grimnjiqe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/grugdmcbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsbdsvkmi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gvimzcxqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqxewypmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkitdafmy.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/geuxxpsxm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gghmqilvr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gyvwphrte.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gpmsxmdxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/ggmfvazay.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gotnpmfsc.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gedeorfgk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gtfyxaqwz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gubbqoomh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gailamdzf.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gvmaowpzv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/glplbdzis.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ghwmobcdq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gimnjzhxp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gxptklimx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gpophwkac.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gfjgvooag.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gnaiylzsz.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxrfwuugq.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gxpfusomm.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gevyruwfo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gjqrevvrr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gcrmyucom.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gcgmfzksh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/ghdolpflc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gqwpzzknm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/getdzeaar.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gqvuaxqhv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gytjwqdvi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gfabfepch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaclexump.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gucfaihqf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gztjplqgm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gxittghck.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gdwlfsuyg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gacohtfha.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/ggpfbrlat.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/ghrnbabha.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gzruvhoig.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gjwghyfqb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gxmmuwqev.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gtfzhomdu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gjrkpxddu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gibsbswvp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtnljrigv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gualfevvv.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtifrryso.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gryykuqsk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/ggxbdssyv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/glbogbzqp.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/guevseljp.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gkydbukim.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gzfnhjaoy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/glscrpvux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gaejajerl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gktubsfnt.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcidkbmsd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gfpymevrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gvpvnavnk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gvbzahbkp.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gmtzbixgm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gnrnbpmcn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/ghclcgqoh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gbmucmyle.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsejlylxs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gqlfgypfz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gcrhopcrh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqgvcacfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gqbnlsvcj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gghsfvdqj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvrfvvubt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ggsubftyw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfardusvp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/geafijvlx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gyuctyosl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmiiblbwf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gsmhferjd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gtsgxxljb.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gatidunma.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsftouuty.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gauzrjnkx.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gwjeztcac.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gzarbrphn.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gtysakjed.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggwjybbpq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gquxwqqnr.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gkksrirbv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gpaiwvyuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gihccavnb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/grcggjuue.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwwplbsdz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gawntapdz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxihnurzw.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gtqmyyaqe.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gpterkuaf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/geksdfefu.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gnzojyfau.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gdbqgrvqn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gxqtsvdti.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gceztptou.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/geilmwbna.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gguofxybi.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gkptoznpt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gjlkwksjy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gzuqhpxrf.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gdgoeskas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gttruprkx.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gdolfoyes.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gfvqkvnzy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/ggybxwovw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/grelermjx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkvvazavu.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gsalkljxf.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gcpzywupx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/grryadsrc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gqnfxlcri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gzjceemsj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gmwjkilgm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ggnapjeuh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gearalijl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/glbsciblv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gtcqmogwp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/genietmjy.sHtML


<!-- 参考信息 -->