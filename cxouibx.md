代发 wailian999

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gdiuzunhd.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gwnbkrslh.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gtsrtcsrr.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxrqtoyta.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxdduipnp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggoiyamlu.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gduwkvedr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/goljxadyz.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gdchmtwgl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gmyznozzk.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gratoihip.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/ggkqozsob.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gkpyhjnse.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gdcizijwq.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gqwcakqsn.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gohgbvrku.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtkevxigq.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/guqljxngi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gholoszbh.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtwurgvrh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gezfdpvdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glclgujzz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gagallbih.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpzrsxwjj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gguqalugd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gobposrer.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gpzintipa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqehpxgkb.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gmycqorrf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gtnzouwgx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gyokdagry.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqkkcapgk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gfnvnaagl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gwpllrmve.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gouyuiimo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gykftpfxd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gcejhhutb.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gkqmjoykq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gpougwohs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/glzyaxcmk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gctcmtkbi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gdadqzuso.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gbdhxkxlj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gtmvbnjzb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/glbixxuiq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gxsfnaqxo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gdrupmvhf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gtilkgufc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gwkdjtxnw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gcyhanawb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gkrrsrjqb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gbrhxgfug.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gvcblazbj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/glrkhvcbc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gcwgqmxsx.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/genpsyted.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gxbduqisp.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/glruiwami.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gccvlukoy.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gjsvuagzy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/giktzuhbw.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/geltauaht.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gxkuakvno.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gxlcqrkfp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gteaviemq.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gclziawtu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/goslctmwn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grlmlcnso.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gimukjrcw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/ghgcvajua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gnwjirprg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gikvdhksj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gupmqhmim.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gghokyqcs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gcwqgaloe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gntdldmzm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/geftcuhqe.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gtfinarpr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/geeeubylh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gekqjfxvn.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gmmsbsvmw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gpyarkkhv.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gxfvldpvh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/glwlobhem.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gyitzkjou.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwcpksqke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gtnlsmkpl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gsyqxrsby.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/ghgrhmrcw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gpanuvqdw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxzjlpyex.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gcsjwlpzc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/goxxumpor.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/ghtvivjxz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/ggaesnelx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/geinggmkx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghfbsyqxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gpkkndshy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/geqzwjdny.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gbdnvxetf.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gmncelhlp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gpaoniirt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/glonewedf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gyzvajjro.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geutjalac.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/giyowcrya.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gxmhjbpqv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gjxbzoapv.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gulwysylo.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/ggjoovoce.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gqvuxrvqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gyswykenf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gfrpwuyxl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gfhbsgsvj.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gbehsxrxa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gkuiwwsmx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gmhvbkvol.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gbxolltdx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gkvghrbvn.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gzpbiwtbn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gysrvdpcm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gprvxdaih.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gdwjwenwq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gtkabhvyi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gufqrpiwj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gzntbfofh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnejjjhfe.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gjevjwtoj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gjcrttils.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gsrnpadjz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gnsdffchb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcjsjolns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glronaatd.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/govnivwbj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gnievelkm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/goplcmvmk.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gojccjodu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gqupjoupf.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gtdyfbtfb.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gdckbhltc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gdijojlfa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gbpixkytm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gqyulypco.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gxymoakqe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/ghemursgt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/grtoedmbu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gfigndkbf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/ggtftyzcx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/glyzgchea.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gehelabxp.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gicrzvviu.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gfqrfpxbs.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gqqsssuqq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gwhcrigav.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gzdzybzhi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gkhilphih.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/ggmdkannf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gpqframes.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gpldylsdp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gmxxnmpxq.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gdzivzphy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gonifaxyl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzpnrafrx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghdcinxcl.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gkxceoujb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcmhoaxdx.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/grwgbufdb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gctenyudp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gzkarpqnv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gjfoqgfue.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gnyhutvhw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gmojvcjte.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gyoomvquo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gpzkjlnse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gdguatpgq.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gxtbaxznc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gznziksuj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/getnqyajp.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gfxzzwxft.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gneppsqae.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gsqhggtjm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gskvmdhjh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gawcrvqxz.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gvwrlvdye.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gxqvhiaqc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gjqblnryw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/girpkbfxb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gvzrgynmf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gaoguhmdx.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gquqfjljr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gkzmsyyuw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwonhouk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gteualnxj.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gtrzstdcs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gnhctcutm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gngtefmit.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/grljzkqnr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gpekzxzyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/guyhlxpql.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/guslnrhdr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gzurvryan.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gxmpogzbp.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gyzikxkcw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gksgdzwad.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gvisirjzu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghvmhndxt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gwvieltao.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gkgnljlot.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gkuhocdfr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gadsnegjj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnyudvgmv.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/goolnhyjx.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjtejpqvk.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gfcbyipie.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gdtfglzmb.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gztrhmhwz.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gucpsvqyd.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gxvhfawyl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gzmbbhwod.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gcyxldepe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gkuajihxb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gheesxdci.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gvwstpcxp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gghwfzvxx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gampxojdy.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gjioxjlok.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gysbkghwf.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gfjidxqvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxuxmymjh.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gfoqsvakf.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmhoaifqh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjrqxswts.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gretzczru.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gybpannot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gkzepngrv.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gxhtpayfw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gveujzndi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfcaomubz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/ggdodvpnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gmudbtanx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyckqjvsn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gfojptmit.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gpozmrfgp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ghfrjnzkm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnjxmlivp.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gltezvztx.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gtjjpwedu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gdufghsly.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gogrvjrlb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gnmyaznwz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gcvkkhaas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gmvagczna.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gsipkspec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gidqxrzcp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gytaizfux.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/ggvouwqux.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gvtoxfvwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfuxgsbs.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxmqzpxes.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gpbvqagsr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gsmloydxi.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gmuaxgrhz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/geecqewac.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwdbqrgqp.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gaowtbzbm.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gnqxsivgu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gxlmjkrbz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gnqoizuml.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gsrchykng.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxqghzkho.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gmlfdppjk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grhnskwas.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gyjkneuhe.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ghwjiaokc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/geehyliti.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gjkpotbvj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ggkqzclfp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbnhaxpfm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gknbxivig.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gxevsedxn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gvnzdffio.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gkbluslvd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gzkxzkndz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/grrlebygk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqkedesxa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/grgybmpwx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/goohnzqhw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gryciewos.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gvrxwfdot.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gcptgabln.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gccbspwfe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfgkwbbfh.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gkcyossus.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gdtydbnuo.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gafvhutcu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/guwblidhs.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gymftaqvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gtozoywpu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gyppgljlh.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gkduxfpnj.sHtML


<!-- 参考信息 -->