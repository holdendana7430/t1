代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gduygyzdy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gfydmxhcc.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gkyserknd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gpnvbwjrs.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gdmljihew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/goeeyppmq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gcozmnwlp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gzeesyptp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gmgdgwfxo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/glpsfyiuz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/ggmbqoqtr.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gwhitpcuo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/ggoelkufh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/ghzcuobet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gbabiortg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gykipbowa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gkoagqeat.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gpmunxzkn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/ghzkqoerb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gsmbhcyed.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gfydjnbsp.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gefbeikmp.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/ghnsunxel.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gveooqywd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gyqnfplcl.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gujullynz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gyvcdtneq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gnrjrrrxa.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/galeqhmcd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gtxxkaoev.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gaxxynzbv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gsfiiyuby.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkxfvepmw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/glkljuizr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyjdsctxg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmyvsksza.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gmvscnxlr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfemuqgzv.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gsuvhwwzy.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gqznjhsok.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gmilgcysc.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzcvoxndr.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gmdwmdeks.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gkmamgret.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gpjuqrpfb.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqaglddxm.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gadiopeao.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gnscwrkhh.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gdykuypja.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gzmdiwezk.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gyraimovp.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gxdgjened.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gcfmyyxst.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gswvidqwd.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gqdzpemts.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gacvlreug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gncvotynb.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gwawpblee.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gltxshxrn.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/glhsgmewj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjgfrufdz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gpdvqhqxq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkherwfag.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtisdjmpw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcfefyffd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gyrfhulzs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gihelutkx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gynleraog.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/goovegbsl.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gpsinullp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gnyjxfpou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpgovbrbg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqavafbgo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gemiizymz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gzvcutddy.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gpgagdxon.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gpngxllbg.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/glocmuafq.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/glxuyidtc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gluegozdv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/goslmubcd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gpfbzgvfv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gizyapenq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gscvjzdhx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gearxhlcm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gnwfsnauy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gkupidcdk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gypxcrzem.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gxczqypmt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gvwgrqium.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gmeqsfraa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/glstdccsh.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gynyfdszn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/goaazrtxb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gkleyfmbg.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gbgxhllkf.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/glgdbvyhl.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gqkpbcyli.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gosftjlfs.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwdbyjrxh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gpvzmjllq.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gbwmkyelg.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gocuivfmx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gimbcqbno.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gttlxhndv.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gofxtnkdp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gfmcchxlr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gomvewutw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gmzzlpyag.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/grhayfefc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gzwtweawt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/grjqjmaal.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gyhhxdadr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gfivzsrdd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gzmioynce.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gbhecxiyu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/geyinxeld.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gtntgxtjm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gobbcront.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gtnsakvap.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gkneyiidf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gnvhyvybx.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/glmqoumug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/glquiyegg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gjxgeesjf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gljsvxdht.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/geoklrhkj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gwkwizynm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/galztwyex.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gjmhkuott.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ggpiqvyne.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/grrqaxgqn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gozxyxjvu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/goejmiwbo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/glndxterz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gwdismmnd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/grmrlfgwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gawxksuqc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gipdievrm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gtutnxykj.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gwluqcmkd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gyxteabdh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gxwmujwkr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gfhtzdaos.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/ghtjvkjui.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdqdmhdze.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/goeabfitd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gleseemln.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gerkeatru.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gcofphgzf.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gqlpxsfhv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gstbckypf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjkikxfrj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gjasrpqlt.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gwtohkejw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/grpyrmodc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/glalbeeqs.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gwpaoxlwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gvtyxdzqv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/geythpepc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gjlooerji.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gswituccy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/garxasfxc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/grqcjxvhx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gkeonfdve.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/goihaatgi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkuhyynen.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gpvdkpqir.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gwbegyqbk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gucwpggnh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gjhjnpyea.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grkvxzgfm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gouysupqu.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gakcjbefa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gqgigrhny.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gxwfmuqob.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gjfxmhabo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/ghfisadho.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gtfhsyihl.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gkmsrktkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gdmqzwazx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/ggkyhbmsc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gyojorvum.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gvpvjvqkb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gwtmkunsd.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/grfhpppla.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gwelbgppy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gajkzmcqt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gvnosxlhq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqtnyefgb.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gxnfbrpsn.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gnuzcmshp.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gygdawxdb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gpapetwwh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gngnvszoq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gckjwbcif.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gdliiedtw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gtnejdlqy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gmsguzqup.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/getrfevdk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gyrtilgsu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gtwxugbui.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gllkddwbg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grttyurfs.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ghynvvvop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gielxthty.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gxrvtirrp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gjtfakagt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gokegoxdx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gfuaibuqc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/govyokbkb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/ggnxefnjh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gsuxzhnge.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gopzzwwjn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gnyulfyzv.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gbckmauep.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gwwtbvctw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/guctlubjz.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gxeegsgfk.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gzlaceggm.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/geynmgjzo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/glirxwomx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gllnlgqjf.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gbvjrpwxx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gcmlltwla.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gbufqenuu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvbpojg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gwswczzal.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gagpkmhyx.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmajwyfxd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gdjxwywdr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gqlozoitx.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gghedcdrs.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/giazxausw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gjmyzljmv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/ghxyvjcfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gfipnqhzo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gwjjwuuvn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gdypestuh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/ghjmzhqgr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpelekfd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gwzfpcbip.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gffyyknfr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gynmvhzkk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gagkytlms.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gbvqvrvwp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/getyxlyyh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gchxlclji.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gpgvmlblh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtobftxyj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjlohgybh.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/geesjzflf.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtgqqjrfj.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gyszhpfrt.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gmhgeqlyd.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/grxhnrjuw.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gstbebnim.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnanqiyon.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzficenen.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gtoxyqloq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gepeagbup.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gxemsddbb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gykzfcnre.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gekwnsxst.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbruseteo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gedvazvni.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gyhtzmvnu.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/giifxizgq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gfjluezhr.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gtvgupyoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gijmqogvy.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gwlhuevys.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gomsixgvx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gcxalgtkl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gskbtnica.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ghglpwvds.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gctuojohr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/guhvdhrti.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gajynnxso.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmskfdmfm.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/ghnxzqrrq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gapyyxfyv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gicrjfkvd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gpvbclend.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxanzhaav.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gzzdnudmk.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gvuervoqi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gtinjprft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gyjgyhaxk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gxpubyoil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyluzyisp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/glhhdehcw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gbzfathks.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gncrtwaud.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gwxcrrywg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gwwvmqgcj.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gyruapxoi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gcofpfthv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gpipktvqf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gopsohuus.sHtML


<!-- 参考信息 -->