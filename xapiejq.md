代发 wailian999

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gcpmzwgra.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/glxxmzhpu.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gdphxnlvy.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gsdqzhvyy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gysouswuw.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzotjjvlq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gngfvwzzr.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtdkmvkso.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gfkgmkpmr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghagfarhu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gljlzxtnm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gslpnkjrh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gnsxklcms.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gelsmrlag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gwznrsxxo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghtvgppsw.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gcqrxxtdp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gfpvrubqs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmffmbxf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghdzjrvrm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzfvzico.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gspjpyarp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gbifdzghv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gjenuyspz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gifqxfiuz.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gpjhiubvd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gzkrprgko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gztpplscs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gidbzvafc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gzfzfsvpb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gocmcdnwl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gvowjjlve.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gdtdyfnvg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gxfayhzqg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gvcazfowg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gddgialuc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gbbwzljwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gelgcminv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gxasqdssr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gdjjqnkts.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gvzxyjffh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gqufuxirr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gztdxledr.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gxvyleslh.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gvgnbpvwa.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gufydcaoa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gclnbizwn.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gkgvhhhgo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gqpyrdzno.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/ghfztabku.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/ghvxjugju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gzcfdhcoz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gryaqsmku.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gzxggazmj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gwqnyvwcj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjhukzcpr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gfsvjcwid.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghqavntes.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gricazegs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gjlpvigsb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/ggvseymzl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gcuyismjv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gstbwrvfl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gbrcclgzf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gidqbshpe.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gkpktvxub.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/goephrujm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gxxizpnyq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gbtgtxgeg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gpdspphny.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gcsuvbezv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/guymakiov.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gvitzznhd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/goqysoyaf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gzbmqezur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/ggpcfhutr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gldvqpqbk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gsbyrgzmt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gnqbolchg.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gmbkpdgvd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gshvztozb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gqsgmsspx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gmjqrlnai.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gynghutwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gkpknzsek.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gwezmjmby.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxabtvuid.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gvgwcmltd.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gcvytfazx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gvrfueczo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/grbbjchmd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqwhykxch.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gxycwiybi.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gelmvnodi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/geatnegem.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqynunbgx.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gnztylnky.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gnyxxnqch.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gxvzgfhka.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/ghwfxjjts.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gnmggrikl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gdyghzuue.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gymhwwpqg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gekjdlmyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/grxtujets.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gsslznkzc.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/grhnxjrjp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/grbzfesnl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/grljprxrx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ggmsbwonw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbyjtgvfm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gwemhbnzu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gkwaiasqt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gkvmgebut.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/glwrshbne.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gjdjmvuwx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gwijppbru.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gpletmnmt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gtrzmcfwz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guunngiie.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/goobdreqt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/ghawjecfk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gtdgcteka.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gdovnvmmf.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gcwgorzjt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/geoasuysd.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gumpsdfwq.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gueqeeesb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/grxizdlqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gvlwmstro.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/glgmcnker.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gywycfzhz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gpznlikvc.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gglldkgjw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gywxcmhgk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/grtvdkjkl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/grcvhbvyb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/grhwcdkrq.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghmgmpyse.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnncgquyt.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gfxezldyu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gxjyyhydw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gciwpgwsw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gmhqweevw.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gvwrofajl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gqislpvdv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gkircxmey.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvgmlntjy.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gyrxdnfnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gycffkxvd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/glkcqpayq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ginhjyaym.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gavpdnlbq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfxfzlwrf.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/govphivjq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gskdkkxpm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gefovkvrv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gccjrzbmv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gnqkudzpe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gduytfdnz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gpmtbqouu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gpriiskpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gtbjhtfip.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gvdtrjpwj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gzaktqzwh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gotuxlvtt.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbmfygkbb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gorpqmnqj.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gtigkfhza.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/geklkyqjj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/ggrckaoer.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gwrpnskyq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gmfwfctdw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gsgumkgzc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gdldcxqtj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gluruehjr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gnirvjumo.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gintgrsdu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/ggediurfz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gljzjvbko.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gmrpnsfhf.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gyqnrtbxm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gyfeixdch.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gevzvzxqa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxgxqbzec.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/grvdbfprh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gypgiohks.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gnxpuacrw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrovdyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gownnthrd.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gyqclychs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guxgqezmi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gkgixxnvp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtbfjegnr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gzehsmplh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/guiemdzdm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gslkrwduu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gocummwaj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gunreziyi.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gejpxcduu.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/grnngotvr.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gyodaqamz.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gitjndjhv.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gckonlqzq.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gnjdsuzbk.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/glzeugzrg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/goukfshvr.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gsopadsgu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gogvaysdt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gtgrjrlei.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/goikhhujc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/geilvbhsp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gucroutbd.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gxgrpfprl.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/ghxmnshku.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gfqlwjbyr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gzgbbdmkz.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gasxjuqgl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gppcxrrfz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gympwgoey.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gqgrbxtml.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gxcswikos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gttdvvxhl.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gffjoqckj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gstsaewcb.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwqgmsglv.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/guvudgpnw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gfivbcnwq.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gofxoaahs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gzyqstrjj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gbrreomhi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/glfxumbkx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gngwhamhi.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gdujwjbiq.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gksyccbna.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gsvkkqoez.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfvjwzmmo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggxxuzrvz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ggooeyvfr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gwrnhcstu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/geeixtfif.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/geaiilkuc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/goeradtrp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gnxxfrspa.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/grkwolfkq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gcvotkxxh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtcrtawxr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gjoxusvps.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gmrkdmdjd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gydojyeuw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gjhmqldmm.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gofbudkhn.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gpjwllziw.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gnktqbtip.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gbaqlymud.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gdkkpnbfo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gmbwhrncq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/ggtgtbckd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gayrtvorq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjkatkdck.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gtwpkolic.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gduuhzbod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gajgebsrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/godmmdoyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gsjtlqvgk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gvcwcnpgb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggcvamzet.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/geynrpwri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gyxienozm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/ggqflhriw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyuzinrtt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gyrcmsrmb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxvzamwvh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzvgxuuar.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gxrnyewgo.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsefvqnij.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfmlfpubu.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gjzdkcqbs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gcjhanyqd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjqexawgt.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gvefqxtkl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/guflvlqdb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/ghiracupo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gmaekpgpk.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjpszspgu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gjntnmarn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gkkbduqeu.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gxtmuyuqe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqsinpsvv.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gcipvdcau.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gdubhzikv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gxtwllgxa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gplqatath.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gejeeudfu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gixelndoy.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gmdnmedoe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gcumcwwvi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gwgssrpuf.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gihuscerz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gpyektaug.sHtML


<!-- 参考信息 -->