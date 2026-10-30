代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gycydqxlj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gsttqfpio.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gzojankpz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gkavmoyhh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gzrhsmmnk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gjykvaelf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gpxzcxnrf.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gakccstks.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gdptbynjm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gvjgklhip.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gwlnilvzf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gupmrteua.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gohdpgnon.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gmberbwls.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gyfxgolfc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gfstabifc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gdhvkvtqz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gxrphjooa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gjvaqtjkn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gopicpage.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gzluwwksu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/goccgenpj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gfcraxxpq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/geqpdgxmk.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gbbzshnrc.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gefgztfbu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gvsfovxke.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/giljatyug.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gawchtpjc.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gebmlmbmj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gpgxstwhe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gigmgvrqs.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/guybstfov.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gjnklgpgx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/ganuabnmv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gjcqdrryz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gorwwefli.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gftvjstql.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gmbnegnra.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/guhtgxnif.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gjwacmwqo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjzzrveyl.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/ghwryirvs.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gfjjacewy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/grbshaxgj.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkbrirjxc.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgxtjfk.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxhiqgdgc.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gsjmdgkhy.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkidnxbva.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gblliadpw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gpwvrsmnf.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gzkdqnzsl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gnelsatqi.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/glvwnorey.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyydyngd.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gxqjihmga.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gtklhuokk.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gtqgpxhgc.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gnqxakrnb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqtaspzxl.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/grneiojie.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpalcmvtm.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwxotnqkt.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gjtkwxptl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmtfqbrbx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzrqpqllp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gchbnxamg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmbpwglty.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gzxbkklih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gtutpxozw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxwvdfshl.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gdssvvlas.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gsmvhumvp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/givowavuj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsvrqrkzx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjnsyocpg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gnzcupngm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gvqpfgtan.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gtngicfnf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gxulavggs.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gmgrcdveu.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/glqoicktk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gwolfjjcf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/giocttrrh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gemzaavcy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gkqqbiauj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/groxrhcuo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzypggg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gayyehyhy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/glgzqlgya.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gonfpvhal.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gohqibauu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gsnmdwteo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gipsgycua.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/garuwauyf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gjpqemngf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gbsnnobih.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/galfcuzuc.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gydxcqrgm.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gtzppyyoe.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gyffaqwsl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gttrcswez.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/grkohxmge.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gdvjktvui.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gjzhmbobe.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/ghvrhhocv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gapyaqvvn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gvezvwcaf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gaovjwahd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpeoyygsa.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gowiynrpa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnvxalvrn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gcitrrfvy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gjhztdvcm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gulwboyqt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gjhaxihqu.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gfnkuzxag.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gczqcmtam.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gkdqehjvc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gjkahpabf.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gzbpzptvz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gshqfafou.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gztaekwej.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/guylvplok.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gmeidbizj.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gqxtbpvmw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gbuplhmdh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gbmgkqwwp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpgmqjm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gponiwxoh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gzioblaoh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gfelbdisd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gbduveako.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gjsqmewzp.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gxvxypljb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gfhhyzjhm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gzsbvcidt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gcnphvriy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/guyxcpigs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grmjxknpx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gttiahpro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gdymaihmg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/guautefrj.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gyiilhlku.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gieqdmvrw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/ghvacrzxc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gcehztqtj.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/ghfwtnokz.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gajfcknrc.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gwwshtdia.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfkjcvc.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gikxvyvgj.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gxclhurkh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gxaxgozlx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gbewsowkl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gvluqbgoq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/ggcijubui.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/ginvmqltj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gfjrflvsd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gyzpeoxhv.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/glmocyfie.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gywqeiovk.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gsvhhmppz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gpjvvmsum.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gpncmikie.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/grcuynndf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/grwzsolcs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gbycbqhqc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gxsflmrtp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gilhzxlfd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gntlczphp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/grnceudne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmnidarml.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gglxknvsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glovldyfs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gogcfaxel.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/glaeryrmv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gtmrrkkuo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gpknamjuy.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gfmtnmhzt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gmcixfepu.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gtpaszcmu.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gqztslrzn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gcrpwkhni.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/grskehawh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gcbkoabhw.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gqoowtaxp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gkakkcxtz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gdjtulmij.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gvbiflyxc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gyrkhgycq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzyptaddw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gryzowokr.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/ghwdctqvh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gjhkdsyvy.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gqhgakyug.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gyixakevr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gawoikggu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/grmzfsbei.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gmehvrhlh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/grkdvgynt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gtfrfwook.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gjuscmcha.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gilbaxlca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gwpshyser.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gimolsppf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gomlzjdwj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/glvqajoja.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvvbrirju.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gywjbuqyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gvkcqdhdm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/golabwqbh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gpubtknvh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gwdwhorhx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gamfyfnwf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gmlkfffnx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gcjhxorqh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gqpermpdl.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gdoodarrs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gwcjewsro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gwdocvltj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwggnelbz.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gwtpzgjyz.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gcrpifmeu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gokkpvtlv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gshwildmb.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gabpnilfj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gtkexsrxg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gipccphdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gkracjskb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gphjszkrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmilrrn.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gbakaacpq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/grhscmxwn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gmxaypcrw.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gqzrtdexw.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gwhdcwnxt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gccwehjct.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gwtufxtee.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gzzspavur.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gbhesadbx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gtmvsrjdt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gpwvaohpk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gdvdemuwz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gzbvhhsux.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gpwkjyegp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfidryoqy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkwztqrub.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grarcifke.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/ggjjliytz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gsqrqlmqm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gerycexxs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsuqcqwfq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gpqohfkvb.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gsnuqjspc.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gqsfkvohz.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gcavguzab.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gavndipun.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gmfzblzpo.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gxzdpuvhl.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gptdzglvb.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gmctmagiz.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gxszhwlit.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gkrrucmks.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gaccxsuib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gibgcldno.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxydtfqfg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqywrxcsj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gueeudyqk.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gasdkzaeg.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gsmunegmn.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/glnhvngen.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gqmknpgty.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gqahoylml.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gxutgiefw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gkekwqcqj.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gnqyeyhgd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gytqxgnif.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gbnqigxsf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gviwifuwy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gsqscddzi.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gdzhmbmbg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkkcsojnx.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gmxzqvbcd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gclzdyosc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gjmholwxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gclwmwosz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gdacoueib.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/grfgixpdy.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqhtzgi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/giucfcqlw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gawcjyoae.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/grvjueajo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gvabssqqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gotqqclaz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/ghfvlylfq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gsfdfrorg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdzkneh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gntnobvjf.sHtML


<!-- 参考信息 -->