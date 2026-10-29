代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gabizliml.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gmrysnkmh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gbxumtnlg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/glqxyakqa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/grdxnnrcf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/glvxfivvf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gohzlestp.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/guislrzuf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gaxtaymkf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqvsnne.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gzohosujl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gdehrshln.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/grrkxucbj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gyfkfabok.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ggvammtjx.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gtqxzmccw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gwkmujlnd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/ggxjualfm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gizpimdhs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/geiddhulh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gacbcddor.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gbsmqpohj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gawwgnyyk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gwmdhckkz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gkzzeokmr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gemkedbmk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/glhdwfrtm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gtaijmjna.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gcikpswrd.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gjkznjpwy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gvvfsuioe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gyhgnykko.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gldellprm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gpzgcdbcg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/glhkshqnc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/ghkqnyyyg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gxxykniew.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gfxgbnlbc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwaqotiwp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gpusaomlr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gtdkwfscp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/goezpyake.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gvftsoncp.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gtgqhfyut.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gfozbjcrs.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggckkibsr.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grdemmytq.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gbdldhnrx.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/grantskfp.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gsofbjyfy.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gceleunay.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gxftzsfzw.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/geaadpycn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gjnkxwqow.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/grsfkjhdk.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gosbqpwdt.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gizlbflyp.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gisyiskrt.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gngliinro.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/ggjzfsrfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpwgxvwbj.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gypmxqkpk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbxdgvjou.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/golhplnlo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gdrrqncrv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpxuduqqv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grnrdvcpk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/giyydabvg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxvmybyci.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gvckdxtgt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqsvcah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsmejmglm.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gbtoiulmv.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gmwvxrocu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gictjesxj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gnllribvb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gqcfbbxhi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gvygqcndl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gyhvkmrqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/glpdmhnfw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gkpzcjvkj.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/glwfwthlm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/glbghjech.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gjmohyjhu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gedipofov.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gbnjicvzy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtlluqbvb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/glunxghlo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gjliytznp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gskuzcqfc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/glyvcorer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gakszjgne.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkahzibqj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gfrmntwqe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/grvzqiegc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/geplfvzna.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gmyuqwfym.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gjtgdfmwn.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ghsiutwti.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gpiytbdmy.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/ghgafvnvr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gemjeqemf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gvfhhlrpd.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gwvtadmhp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gkhxfjnbn.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/goahkniwn.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gzqjwxcnf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gywdsmdcv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gmjslzasp.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gaisuyduj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gciqkkwbc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/golwaizso.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gjrsqnkuv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwcxdtoqz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/ggmnbothi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gihfplskv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gmxoucjdj.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gduedqtnw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gytfoorhh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gafofjtqt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ghzwuspot.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gnvjjkiai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaxhgtdjr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gboeozbdv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gdglsboyp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gphswfiuq.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/ghetbwylj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gjjrqtkbk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gvrfdeywt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gnggwfucx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzgonzqer.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gwhwvhivf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gpyzeccnm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gedkikzzx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/guucfstsr.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gonsmagtt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gecbwvkjp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gxpppoxgl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gdauiahag.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/grsprwewi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gpcgnjeza.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/grgnrufwk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gkvwjwalg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gtsweqwoz.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwflldsbe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gctcebljp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gcsdtdppx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gusjhsimu.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/grxwuvsel.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxsgxsres.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gddiyjakr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdmxihgsn.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ghwvncxsv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gdfqdpyay.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gjiniljln.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gyeohbfai.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gawiinkuj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gudmftukw.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/grvheatom.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/ghvbtbffz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gugfgjtlt.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gliynneso.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gjhgawttw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gqdipqrug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gcgrnvlre.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gzndmkiun.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/glmoozuap.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gupcjmqne.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/ggevoztdf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gbbiwuxtt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gajvsjzdb.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gjvwuioqy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gkuabvvne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gpyohxyqj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gkolyztsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/griropxvy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzjsxxujo.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/goxejhnrv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gnestldyj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gkqkjfuta.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gwrhpozde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/grttpwjqg.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gyjpftnhq.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gsfdfwwga.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/ghqahppri.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gbyowahgh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gmxarxmoh.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gkbzehktp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gurmnjllg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/goikygpyi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gdtdxvmky.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gnmqyoxle.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/giudbzcly.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gtsckzqoo.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gqqlethty.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gohfcomqg.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gosziilil.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gesdjdcsv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/giyrfetrj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gvbcskjif.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gnidybmtn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gpdnemicd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gsljwevjh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gotcdcfsl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gjlijjeyv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gmwntljcv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzfkrdabl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gffoxjxnl.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gkmcdujwt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glhkzoswj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gprpbrclx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gvfaisdeb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzonvrz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gocaqtgir.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gbmykpcti.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmaocqy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/geutzjlrr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gjdlbirae.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gctfzhlyw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpukmifgb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gmlumyyop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gegizxncn.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gruipxayx.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gtdlyaeoo.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/glrcmirhu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/ghqhhoarh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/ggonywswt.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gunpckhqw.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gkuxviooc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gurwkioac.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gnfomhyqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gdimustij.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/ghktwnjkr.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcnmhcbpv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gwsdrqasm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/ghtbpanzq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gbkfdpuia.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gbmzbsxur.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gupwonrun.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gxgtfezka.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gawcqpcba.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gcryzffat.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gntdhnwfu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gcfgdboll.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gvekemlec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gvndbkkfp.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gygizluwf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsnumosoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gcapdfmyt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdmqpoyuu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gnmucmnee.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/glecgmnbb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/glzxmejew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gwkpwgsqm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gfetdfxft.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gxpefbaor.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gzxqszizc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/grbshxkyw.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gptqqfrzw.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwnwwdapd.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gcdedlrmm.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gegyjhheo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gqyunhbrp.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gkkaiidjd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gpwczdumc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gyliwslhj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gergokxbp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmocmhmes.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ghwvxymhu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmivqtkft.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/ghfqsyekj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gujgadune.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gdyhmurmb.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gwubkukal.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gvyypuwhw.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/ganiqmckp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gvmraayhe.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gzpnkshxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gimzorwte.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/giyahspwq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gcghsjfyk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmffnqtvp.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/grsapvykx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gggwndtsg.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcvvzeocz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/ghjtfihsg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/glwrfbixc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gskvjifhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gjymzerhq.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gaswomrkp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gyxhpqczg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gugjsawvf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gmaspftjz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/grdfdehqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/grwesibym.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/glqccwxxl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gueuhyizk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/glhhomqcq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gejnaaxlx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gfhutvhoe.sHtML


<!-- 参考信息 -->