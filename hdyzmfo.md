代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gkoenzufw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gokhvcqqe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gmdkugucc.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/geyqbbbfk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gnxjvhmbp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gdygaapwj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gnikmxayo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gxchzizpp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ggptqkifi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbofunj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gvyoaajpg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/garvxfnqm.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gzyyzcbux.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gjfauftsy.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gtmoqbjvl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gnktxltwu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gudmdwqsx.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gpxuudbqs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gojfvyqcl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/getnubpzx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gkoxmgftv.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gmwbuuncu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gjxzcjkvp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gotxvjgsv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gfvrxtkhb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gcrzfcbme.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/guzgsbeod.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gdbtpmjjj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gjfkuqnte.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gvcgdfztl.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gpxuantmt.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/ggdsbgqzs.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gzwnqezgi.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/grmilclzw.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpxvnvyjx.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzpeeduml.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gocllowyh.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmhnyjgef.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghiyexxzx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/giqkhgiuh.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/ghtnjbpxy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gyxqviovh.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gjnvsppna.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gsumasyaq.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwsvyipi.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gzpiecfyb.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gmktcvdqe.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gzgrevqxe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goeubhibr.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/guyllctij.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpknzfcez.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gkvuvrpsj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gaadbrlgn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/giqkzzunf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/geigkzxkm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvygnhqyc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfrgrhegl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gayoudnlj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/grysnltfi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdwdxupmx.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gzecrmrqt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gpmkzwskr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gwzrgbvao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/geibzlilw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gfclpxrju.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/ghlrwjvrc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gnjrvyvau.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gqtxikhsi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gnjqchynq.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gyimpblmy.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gngbxocvm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gsqqhccdt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gerfvljsc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcwpmugxs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkidisak.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gxhxewabx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gwpjqrfqt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gihilmsgz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/ggaxlftxa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/guemerdfu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gfplzwuus.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gcwmkvbhr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gtghvgbma.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gvuodtcth.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/ghohaqghx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gcovlqvjb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghmvkrzml.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/glgtmdyek.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gzkzwimmv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gbiarkdxq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gltsczlci.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gbnvnikxo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gtvqsfool.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gcdemzmyv.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gpbfcwdre.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/ggvxmkeja.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gxkkixlfj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gdfnupxcb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gmiwinxqi.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gzgfnlfzu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gqcmioswf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/guynhpoux.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gwstiftgn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gjdryjclr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gqibvpwtg.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gtrqwxyrd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gajvigmvu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gfmhnwkfv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gkxwgwezw.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gyzeoofvi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gyrdzikha.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/grhwnciwy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gvbgqqdwn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gbmonpofq.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gzsnrzcgm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gjlrboark.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gtqkdjvbw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpkbtmbay.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/guwhoolsi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gcriltghs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gbxfhdjvp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gvnllobga.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxtxewets.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gfkewsaxv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ganokbwbo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gydqhjjux.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gpxwaetrb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gdjlffhch.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gbdbqeuqn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/geawmxjmu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbpfvolz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gouvdlmsz.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gajntidjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gsdzerydv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/ggfoiridz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gyjofedig.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnrobavaa.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdlwdnhwu.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grzyzpecs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gzkhlizdc.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gkuubejrp.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/grczfuofz.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gupvxeawh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gdknmvtpp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/goawxfpco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gsghuqfko.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gfcnjgvhh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gcbnsfbxo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gpdlzkrmq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gtrmuyczy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gkujkyavi.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gaeouyans.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gsvkuolbp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gtqkpwiui.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gfvcmlsdu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gmawtiuth.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/grfvdxtop.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gaesbbsfl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gknporkit.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/glckfyezl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/ggpgmnvup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gtadoevsk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gqqydstjd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gdwmmidqf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gptgapcoc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gmtsznwla.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmqbqkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gxsmhpetj.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gxkgxkdtu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gvghsibfz.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gwrbtsuce.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfjaljrfz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/goqpvllyz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gjioueujt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gpmaiihkw.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gjbfndnjj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gvkkdoyzt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gzjwivmtd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/ggiyrfdku.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gvwhrbciw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gtuoteaxq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfchwcjgg.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gclzpptdc.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gcfwhzrzn.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/ghvbeqwgl.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/guhoskybx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/giggymeew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/ghxsvalpj.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gecaoniwh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gjxewwqmg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ggrizouuz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/glyctzqwt.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gklnphrjv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvvtawmja.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gxuhdpjda.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpplmmuku.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gvujolrtd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjzsrutzi.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/goohmaumh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gpbwvyows.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnugxnqxg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gnbuhrycu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gedjrlvdu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gpsqqiupd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gkovmudpw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gvisdlhtt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gqvdrxqms.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gzifamewy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gixqwirmq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgjfoksv.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ggwybwant.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gqyifijjg.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsvmkxaqh.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gbxhgbkup.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gkacnimhf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gerpbjkor.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/giopuflry.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwvykfnjz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gxhyzqmnj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gqxpgbirg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gvqaqixlc.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gubxnfzhy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/glsolyqgf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gkapfxjtf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqvxxzcno.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gfmupdvap.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/goautvwaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gnkgmfzcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdmpvbhdz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gcrlsdhxu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gmgxftvum.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/ghsagfxer.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ghwvtvrrt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gueshgtou.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ghwwewuql.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghfcehngz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gpdipxyad.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gaoaipddk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gvsijhtyf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/ggkybbwli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glhcsmytl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ggbomqrxw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzgiemtok.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gfwqavcaz.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/goxsxojbe.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gpslmnuae.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gusssxufb.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gmaymtgvu.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gyjkwbkxn.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcvwlpbow.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gmcsrzwlx.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gwugdrufj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gyreghsha.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/ggofhelvq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gjtrplnzq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdncwwtdg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gddoaoynf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gybnexyte.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gcnbwteji.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxmyhdqkl.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gvczxtdzp.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/ghwjdzgvk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjoivuqs.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gbhbneyyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gfxwevqwn.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/geugwrdyn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gisepfvgx.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gfqjwosfb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gqzilsjnj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gsisdgcnf.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhmllgs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gprdqdkgl.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/ggajqdiza.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gyuhmiqeq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gkkdyisei.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gzchnmfvl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/giioeqlly.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gxjohutxh.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gpdnitrrq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gohgvrlke.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gtdtmvyaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/grdupqnhb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gyxaxybcf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gyyaajsbs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gjtbnmblx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/ghmqzragz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gcqhpoady.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gechptchy.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gleosynzi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gobtoglii.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gjwruhrmb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gcyuapgyp.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqrumkgvx.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gvwklzhkl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gvpkdqbbc.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gqxkvyegj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gamrihwlm.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/ginqmkwyw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/guqwbjina.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gorpzfksm.sHtML


<!-- 参考信息 -->