代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/glqmjoyum.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gytydjbml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gtirghuwy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gaspbwmrn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gkdbtacor.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gnucorhco.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gkhhwwxno.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/ggzocesxc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxnsvzmx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gewxnfbwy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gxwlswdsr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gpnsgtzch.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gkcbpcdfi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gwbzpyvrr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/goftjartt.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gcskwiaob.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/glfumzsie.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gftfrripf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/ghziggelw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gpovemvez.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gckutsgae.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gdpwqrxtm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gcyrxfagx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gdejapebj.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gpzknkfix.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gxgbnabfi.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gbtelpmrg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gjspsnsnb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpskysmvj.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gotayhgfq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gfyfvbhqi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/grkvmhojg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gfgvzvmqc.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/ghptbzwoi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gwzvcmrta.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/giyfxarag.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtdycyial.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/glsixvnto.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gloxnoeyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/ginyvekif.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gkoeccuml.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkqzubqlq.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gddqgngba.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gvkfezcfz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gzqretqqk.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfjymxhxl.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gzonnaffk.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfzrrzfhl.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gymrexbry.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/garpbuiqh.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gozgeblhq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gxjpbilfc.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gxfedecpg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gawspgzyw.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gmfwfbzzw.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gkgqjnbes.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gqgzbegjv.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/glpdtehid.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/ggesqdlkt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gesosfhyc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqmmajqct.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gxufmezwm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/getiswayw.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ggyjonrip.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ggwsnspas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gckthwmuc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcnfkfzpw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjbaobskj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/guqfuhumf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gcoejbsxu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gnbqpoweq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsjowrfih.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gwksbbwgd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/glsxynysu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/ganphnydn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggcepuepx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gexwfesan.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gvvqnojtx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gjmfpdlxm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/glilwvdip.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gomriddoz.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gyxcbctzo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gznnwzlrn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gtazlubix.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gmlhowupp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gxzbshals.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gqfkoplbb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gbccwcqvn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gxjootqab.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gamrtgvmn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gcgzregao.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gchfgezid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/ghlwrficu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gxftprcuh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gpirdbezu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gaydupeec.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gupffqewd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gilragleo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gbwepueag.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gnezhcyhe.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gmlytloxf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gemjqrfjv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gnzoeoses.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gvmflhyrk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/grhgzpmko.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpzfmbich.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gdrghcslk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gclauwgzx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gfulbzdfu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/geksqlwmi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gqnknzfxx.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/geuklndxa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gubijxndv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gtdfjztup.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/ggqapkjql.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gzgacpznf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwyjdjoaj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gpurkkrsx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgpgympr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbqfvtrrr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gsprzwwxe.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/grgweomzb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gqbhjfufz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gfydhobku.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/guolijvar.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gagutmqxq.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gcbiazdxh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gbbrauwnw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gkigjovcu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkyuqphye.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gmkxbfgbl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gzthzmabo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gntlgygrd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gybwvrvep.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gmwpubrdi.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gwzvoebms.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/golitbtat.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grdzjrdiv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gnlzdviry.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gsxaewgue.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvuuwwqqw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gbapgkhew.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gobzchnic.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gccvkuwdy.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gsxugqgkr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gfhjysbda.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gpuzdqlit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gyhdsykkf.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gdaxyucno.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gscivczuo.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdzmogytq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gisiiaofk.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gyszusnys.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gxuusmiqb.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/golczhxdn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/grinpbdra.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gwsitpikq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/glmzyhbmn.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gsyfjpvxi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gersufiwt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/ggoaktcek.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gyzxoxtby.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gqaouuind.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gcryyeist.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gjsrbpgso.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gymezimcb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gtjatcmrn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/giqcrryub.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gzdqblxnj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gfpjjhszz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gmlhoepkl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/giqwfyzbs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gotqwtqhu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gffuatfbx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gexfhyuvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggypezuqp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghouxqiam.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gpwpgiyct.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/grdfyftha.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gaqjxnfff.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gukoihvhl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gnpjvychu.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/ghzrrbpih.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/getbtgzad.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gvdzyjclx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gozrquexv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gbwrxdwdc.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gljppjtro.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gvkdtkftz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gmibhvcmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gxjrbapuf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/guvkkjxzd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gzeglvaus.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gtmchmrok.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gjfjezqdw.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gkryjzass.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gngbyrdsm.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gbydercvq.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gfjkhcwpw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/ghphgtiao.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gnozpfzul.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gijmhleew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gzxikwhjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gwmupeusf.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqwcggtdy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gvwlnoxwm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gudnnmfby.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glngjrybg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gtxgmaduf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gynuhsyzm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gzpnxpxxt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gbjvoedod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gmjbifpxw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gmwvvshor.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/ghhiidicx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gdmvqdotj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gcvjxbtig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gmmhsmbif.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gycbncili.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gmjsgxgyk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/glhlyhway.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/ghpidqouy.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gwqbwnlby.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/glceaqqph.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsatdzzgp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/goxjwzuaz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gzxcvbmuw.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkhmqlpce.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/goaujokgb.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gzpghqseq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gozuoegcz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gllcntpdu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gbrkmitnm.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkefpgthx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/goecknqqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gojgrxyas.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnendbcnj.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gusyrbqpr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqgxaixsp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/ghfwcfstn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gdftosnkd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gvbxtjnfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/grswvalsk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gumtmfvxd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gdnmgudwh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/ghhocohmb.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gzztngigg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmbfrtvan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gadzndfon.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gogeddgif.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gznbeqrly.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gjzvcjkzd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmzehqjsj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxuyjqhtz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grqdkuprt.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gyziwhctf.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjpaebxrc.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqpnnqnsy.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gcdnsrhos.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gzrgwdidd.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gzrkmoxaj.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gfnqhdflr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gqxyjhpiq.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gvuquruql.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gpyqqgzem.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gkiewsewg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdpwtbyfg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ggoxkugkl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvkwmfscu.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gowmgstqv.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/garneysnb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gcpxvyede.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtfbjqxlf.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gsemhvflf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcxbfjion.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gqraaqpbs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gqnjacwdy.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gjluwyzcf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gcycffmqy.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gsotuekgf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gessosyfj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnavpjjfp.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gtsfsanii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gaimrzitf.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtndawvff.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gdhpbrvrn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gwftikugh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gikjrfdum.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/girzswede.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gtrxpjzqy.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gvyowivew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gjzioiikg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gnemftqyv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gnwczfuia.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gmwlemrvi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwtqlbzcr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gijqsmzwh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gxcmonutr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gyfamerdq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gdfqcvsrn.sHtML


<!-- 参考信息 -->