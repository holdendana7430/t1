代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvcwzlp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsqviiic.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqctorhru.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzuxkpwi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/grjmhyzrc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfddasoh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfxqrdrk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnabtzcdf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthrrhuwg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfjopxiyu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gqvauxryc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvheehhk.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/glqxanbnx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufryuksq.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqomxggo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtppltiq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgfimvb.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywibkhe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrywzbsu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/girgssxwd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gibtsiagm.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/gqaihrrmi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmmnzhof.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkehnicra.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffqkmsuz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdreoroa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddemctqv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisjomim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmmqgya.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwbglzwv.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlgkndtt.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gskotgvph.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikpsvrw.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrtsfdud.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gmticbssr.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gkzejjsem.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gbggrirqa.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gnlzftuyf.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/ggtqfsnnh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gnctscnqm.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gugnevwpg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gputnmokg.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxpqail.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmczmdtg.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjvzkent.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkpjmucf.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/groqzjrgl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpkwkwii.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/groktkgbl.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdmndudm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmwotkm.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfgxrwdo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/guobrobjl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtazkuhpk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthmihvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynbjgzhe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbqgpxmw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/glwmfglur.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwttccoyc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswjrvveb.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtfdjyaph.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjvkdhwk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkbibhud.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gemezuoxq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpssuds.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gezsgwnnj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gspiaeohr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gyidxkyzo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbqzbox.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvptnjzh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbhngdef.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/glcwiedvg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzxudslt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfamzmtq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbnypnrw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzmksihg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gesmnboey.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gjbgtvacq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grsyrwmfl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkwvmnbo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggldwfhnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnbmmcs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gyzftsohl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnicedonm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbjcwoxs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtinqxwhj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmdqmilx.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiztiugq.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/golzigheb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcayqhg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmmkzybl.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiyfgkaq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gcbwrvoxe.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkscfpe.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbyacjcn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/grzvgiqmq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntdwdjdt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhpcbztz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fanxiaobao.xyz/Article/details/grwebvucr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcztuwxie.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gqoeovxku.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngcuslgz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjrhfrqa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/geeozcjsj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/giyqdvxbr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gmjsdwbix.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gmbunlfbd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaupsievx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggphlkdgg.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudzzogx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gaqcravss.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/germkbmme.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fanxiaobao.xyz/Article/details/grkpwmcab.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gpxlbfktn.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gwllledrh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fanxiaobao.xyz/Article/details/guglnjcok.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gghbikauc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxchhpyk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqvhdgrw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/grjipwusl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfenuknr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtnmfmc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grobmrlvr.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmsvujtj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gytdgatrm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwykjtpzz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gznnqmbuy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/ghjmfnxmu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdagmvbz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjrlhmpj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqpsphozu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzuauma.sHtML

[C10] 变量作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeqabvul.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gbpwsrvfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gsxmbkaeh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsohbhpb.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdygyiev.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxernrhy.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gyipteidi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjrhqqiu.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrukzryt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmpwbygj.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwadrcyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjomvrlgh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gssskxrqp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiucyzge.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/gafcignvk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/gpammorif.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/gnmyyqqfb.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiscqzed.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gwkysutpb.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/gbevxtgcj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gllhqgkfg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/geoyfmblu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbncdthtg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxbmkmys.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcjcntt.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gpdlqmczl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galcvtvbx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsckqdwp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkvqdzsx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdeaculri.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gvipbkwzk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkyggkus.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxnfhzwzs.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdzaclm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvyxvyab.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gyjjyatex.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gubbpgocc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghacupulm.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfglxekhb.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gqnmsheqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxckymup.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gullyczlh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfperacs.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/glduyfoar.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/golxywybn.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwodaurs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gcmzygicm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcpoicxt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gugyodmvi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffmmjmnk.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gafmpyxqr.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqeawuct.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gigjzunfj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewojvdvd.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/gesdqrnyl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/glfawvrgv.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqhthswc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxprvokm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaebkied.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmllyjtmh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/gsmmdbkon.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvblvkbl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvglugeqb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grzhevyeb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gvabcwbwe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiuljooj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gwpwinxdw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmqvxut.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/ghalmuecm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gihhiwtbg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyloinvds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/gfusvxsal.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/glsegpvbd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghysoidjs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapdzcui.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/geuqbtlfw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/gnvjiofdl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxiiapb.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhtxrncc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebnlnyob.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqwmiwfre.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/giexzkcid.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknldvrjh.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gphuqrzvj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtsnqcsop.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbovmazrq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhooxxcx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gjviumwnm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnefcdota.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqafxsza.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpicjmhnn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhwbwmj.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhlnmxcm.sHtML

[D04] 删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvioccwaj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrsqduok.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmoslsxs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/grrtbviin.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxyqidgn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsnamyb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genegwoze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdajvuftg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwfyoksh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbbvntzj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyzlhuua.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjsgxkax.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuuzsqke.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhtfompp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gsyuzpvjx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gzriyixsm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gsudhzjto.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glttjujuz.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gftnncfcy.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfxjrnah.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gpokhoupq.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gstiiaeaq.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqeetcm.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbkvodzt.sHtML

Go:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gkdjvdcnl.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeacybyx.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyoqaxnf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaypzqaw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fanxiaobao.xyz/Article/details/gocynpivt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuugmzco.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/guuqibwpy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezelaayz.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkacckqdi.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/gmcpygqag.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwqzvej.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkvxtvjg.sHtML

[D08] 合并两个数组
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtdzxds.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttalitd.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gewzmttir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/galogcmcu.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gddfsmeeq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkinvmkn.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gashpatmh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gebekziaf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflgzovt.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfezcutbk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gekxyvsyj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxdxaji.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcmguuxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/ggjmclfnv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnozusha.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoqvpnhg.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkvasvjc.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gnofvsgjy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/gptiqdyrl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gnbuhyygz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyeldaep.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gndmrnfsn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhkcormi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcqvahwu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fanxiaobao.xyz/Article/details/gicodswhs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvwqrfab.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/ggmjukbfn.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gszdwkjec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/gwefymcpm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtbkkiv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gebctqxpk.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gygmmguxi.sHtML

Java: Collections.reverse(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gajcfqvzr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwtmhbxu.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqrgfzmk.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmcwjkrt.sHtML

[D12] 查找元素下标
来源：http://blog.fanxiaobao.xyz/Article/details/gmoamjvrj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/goybsmuxs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfqcfame.sHtML


<!-- 参考信息 -->