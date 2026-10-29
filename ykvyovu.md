代发 wailian999

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gjfhreipn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gczrttkyb.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gizfgnnlu.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gzowlgasl.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfyxkns.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gdwqgumrv.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gfliqnsdm.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggovsanpa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gearzoywy.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gdlrmiphd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghxsekqqr.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gophfxyih.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gntqnzjmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkueozihj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkzsfkdap.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gpjpcnguv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcvrvdlyp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gkkegmgaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/guuiclouj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gccybdlzv.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gygcwwxhn.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gdthfxnar.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gdtpfuchl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gfffiajrv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/ghgtrqsvt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gxunmyoii.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gvtzzqkcd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gzptdnxje.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gqxrubqll.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gyljaqdfk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gjlkhgehk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gmgiehvbq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gasiekxaf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gesawbbmk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzhdixsfb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gpvaqwsyw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gujzuagph.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gekbtpkkv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gvzgklpbf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gkerdjtqr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gwnvqfjtf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gfvknnvpn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gwliuqxqs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gleirorrp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/goafveaiu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gumlmtcww.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ghjfvlpko.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gcsqwkogx.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gpfczsmha.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gbylolsok.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gwepppqfr.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gccbgokxl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gqcezrmtv.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gahgnawhg.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/ggniysaxl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gtbbnirow.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/guvhnuodd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gmoxrombh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gldvtmkfi.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxtivrrtn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gusftlxnv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gtrmfmqpv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gzdsvkxup.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/geweugixu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gwayosont.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gywfoutdn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gqnyfbwvd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghfraldkx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/ggqwfkpvc.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/georzuxvo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/ggepbcwea.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gmjhvcvmj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gjdepplfs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/guniskpkq.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gvonodigw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gsxquazim.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gqllwmujy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grsbjzzne.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/grvatkkip.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gouyxhxhq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gfeotoyoj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gomdcbgcr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gljxcwqju.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gkvytpsle.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gycmnjlmr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gyvbxdvcn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ggzbazzfd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/geuznhzgu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gbaculryt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/ginrtznxm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtgcsmgwh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/ggiahwvrv.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gckwjqowz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gwhirqvwj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gjpscexas.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gussuuowi.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gjchvukto.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gepeolfwo.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gpynqnuhs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gpnxstdtr.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/glqypznjw.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gfwaraans.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gloaxtdzd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/ghtozaqnq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gsrwemvpa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gnmpitrte.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gbzwjfkys.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gaxecmzud.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/glxwzorlz.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gkaiuviyz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/geydqmozl.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/ggwghpyxb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/glzycvvcn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gnxwximoh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gluxijmwg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gqacmuiat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gpknibosb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/geruywych.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gmmuieusa.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gytowbxzm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/geuxefkav.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gycgrdqrb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gupbbighc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gkxgceuzx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gchjsijnv.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gmihkgfis.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gspxwhnwy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gtxdeuaza.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/glayfhvfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gekgzonrx.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gigegpyvr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gpvobmgqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gmjdpfjxi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwxyqxl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gdemiwevv.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gcdfzfxyu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/grgaxnebo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/grolyllxe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gbzyczmig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gwkrmvuew.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gcohtvvmt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gtpengrpr.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gvykbjlsn.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gondndarn.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gtokulklc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gmmgbkpjc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gqkizksnc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gvmhnsurp.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gkxmjcqrh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gwevsfais.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gnllvxqmz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gmlvhtany.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/ggizqcpkh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gxaslefah.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gftdpfltl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmogtqnop.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gusiebndq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbtxxtpfy.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gfegsyxdb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gpomihtat.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/giowwnigv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/geyutldlb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/guvrjhujd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gbjajdrwl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gcnmnqpbe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gmxipcdty.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gkyedhbik.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/grfipphfr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gmhakdsqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/ggcquigll.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gtqdvfvgq.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gbvimmqyc.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gahkoucyi.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gleggwhlt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gsuriwdgr.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gmfnnnbbv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gdxifaipl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gxfwwcjqk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gbwnoeoli.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/ghrfgvnuz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gqnmbtfig.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gpqaazvmq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gnjmbvpue.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gnltuipgw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gnktylvuz.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsepdfien.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gcvookppz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxompsxum.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ggudzjpwg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gkwuhkrwq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlyenec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/ggcamkuwp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gwneokwzu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gicxccrcc.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gjhgyjnrd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/goyxbmmrm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/geztexkrv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gnjouyvcd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gyzdyvfar.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gxhutclce.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/groejkhyx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grathjblb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gicdendat.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gnjchaqcy.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gnubppmws.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/giacjbyjh.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gintgddjf.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gfzeisvuw.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gqmranbnj.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gaoazehif.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gdqrdmjnu.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gluhcikkz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gbieotqul.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/goiyntmjo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqvcozrum.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdioefpvz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpvewulvx.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmeytqhvi.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/ggccwzmnw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gxdwxnkip.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxfcjablr.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gexfxlkul.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gzxpimrfu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gnakykhra.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gokfofdpf.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gdribnyaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/grxiwmyca.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gesfimctw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghuycwmso.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glpjkasrk.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gzuwmafsc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gefqnmdcr.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gbwmturgc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gpyzxnlyh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gjmiufjpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/getsrvbhy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwyaoqdom.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gaizrsaqf.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gbfltoxcy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gfeqfkirl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gneabcpng.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ggydudyyu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gsztqjdwi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gguxlwgwl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/ggwdqmrjl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gmsmtiqkf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gagwbcgvx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/guqjvjejv.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gaayjrjkz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gjdkdvoit.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gjhkyjhou.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gkluhqqrm.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gzzzfweuk.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/grwfvafax.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggkowatbe.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gyoaqujbw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gyxirgdpq.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtixegtus.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gnuhzyjki.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gbjvtihrc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gvpkblcua.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gximvkqzp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gqoewmxte.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbtappkiz.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/glngcnazx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gjgjxckrk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/ghelaycvx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gwwjzliyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gcdlzvsyk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gkpoircrb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gyfbcylsp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/grjcsosrq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gzvkzgwsv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gugxdnqob.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzevggzyv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gdvtmgcgg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/ghefgfniy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gozrafdhp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gnwxijsrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/glaxewdui.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gkphlqeee.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/glbwgqzlp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcqvufsfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjonpnazj.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gfokskfua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geuarskxp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gyskhjgtj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gdpwqiyop.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gyjnwfnoi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gdqwebrkw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gjdnjwpui.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gollelftb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/guwzowwaa.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gxezfogxo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnoyktta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gyjmjuked.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gfjgviyhz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gtukqknzc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gxtcdlqts.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gimhgsnxy.sHtML


<!-- 参考信息 -->