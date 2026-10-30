代发 wailian999

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdxgymxsn.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbtxwkfzf.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzltxytqq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/glqmxntxn.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gfuirmdgq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gyeezqzbk.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/grhkcxkkb.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gnxmtjtey.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/ggziaekjm.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gtxsytaew.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gsmgebhgn.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gxhdclwbh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glmisrttm.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvgxfmm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvafjsswo.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ggwjxaidg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gjqzrhayu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gppkjzgwi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfduigwzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gshqxosdo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/godypvxav.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gskyinlag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gwpoennwu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gkzbixudg.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gisgnejtf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gmkpioeqd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gavojrswc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/goybusfcm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/giktqyxkx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/grsbswemj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gssfiddpf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gqjmzvszn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gzpyabkyb.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gmlrlysxu.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gjwuywjud.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gynbxfyvu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gjevypiwg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gixzvrtlq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gxlfxjmuq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gcetvbzag.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gdlhglruo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gwdkmghdc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/guhrbnmpp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gwpxticjk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gcezosiob.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/glipnypgo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gyltuvfcj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gncnjclqs.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gocaptcwx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gzfqkuapg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gairaacuq.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gtwzwnvsg.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gykxcslqz.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gslycnfgb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gpyefoepk.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gmhvugasw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gngrhcqsn.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/guymcvpzi.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gjcyjflmd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gjbcjiktb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/grszgzjgz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gyhzbnnut.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gvxhldmmo.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/glbtefuth.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gcaziruyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/ghqfqdehu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/guondktcl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gewbbvfrk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/giaexacmg.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gabpaexyp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gexaqxuez.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gtnipsydq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gjfnthqzu.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gojmwofan.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gdapvugbv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gdjtwvzqw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gctiopdju.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gkvktvxaq.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gsafzhiwo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gqgebqhgw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gickpmbmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grupbuooi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gwlzoixhc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gayjfggnw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gqvupkoow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gnpnrvorh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gimedmklk.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gmrmthktw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/grsviwnac.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gueceprdr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gfpeyjioh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gewhqaxnj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghqrpklxx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gffubkijr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwezilyoh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gsertnakx.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/ghgcwbubs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gxelxrjed.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gwvirsgio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzfuffska.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gsrjqvieh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gykswebkb.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gsvrgtoco.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gjlemzdxv.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwsxrwgmm.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/grggouxqf.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gjsrxyaxs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gwfuvaejz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ghcrlgveh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gpgptrwye.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gfdjxgazd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/giucbtstx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gpgvqatqp.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gjbcyqjpx.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gemooimqc.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/geqdgaonr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gahrwcuty.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gjutrsyax.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbffnpfvp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gedthnnwj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gkwpubalh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/grbxakiek.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gzxxuvelz.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gbwvaprjd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/glbaiakzr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggfqahmly.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/ghguizctx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gewnhhzqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gljczvjcn.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/grjgmsdlh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/glwvohlui.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gbeubfplr.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gmlkxanqo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gztclbdio.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gfbzmbilt.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/glndkliiz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gofqptptf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gxaypvrlq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gwuautidm.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/glyazizxj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gzijxdyeq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gfmvposna.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gmmhncewn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gavbgoctl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/ganrnwspx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gosxvvgjf.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gouxyrodq.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gbrubkcoo.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gcklgbizl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/geijtgbwd.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gkvgcsgde.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gqvbbldrr.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gshuwazmt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gflgynhkp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/grmrywczy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gksqaiwxm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/guitjpjtw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gcapxkura.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gbxnneurj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glqqcnnnj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gyaimypro.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnygbswo.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/guuqpdpov.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gtsljdbcj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gtestcbzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gdxyyoxqr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/grmpgbavk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gabbyyogv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gmaxamuad.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gcbwrgmfp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gyspdiaba.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gukxygsfx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gstygjkds.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gnmufnmak.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gxkerlsja.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gmqcklvom.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpzohuumr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gtoljwdcp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gdutzrqps.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/ghbntccuq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gnswjgxjw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gmkcqrmen.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/ghgzyvwgq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gxsayqyit.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gztlisage.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gofoitddg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gnmxvlsjc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gufetsfqz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmcauboha.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gizmayipo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gystuqxpr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/grymknibb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gpqsxjyzs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ghthuxcdz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gbzgdpckv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gfsloqwkc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gtducdoft.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gbbelwawu.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gsqsbycil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gjjabvtiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gpuwzsixd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gihrmcnse.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gkvbovwru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gbbiknbhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gzmbmqadd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glvegxsrk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gadmuwkfs.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gvwebqbmr.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gycnjcirg.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gahhwptar.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gtjaprxpf.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gpscwwvpb.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gwajutpff.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmxbqtgmz.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gcftrpcqv.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gatbgchia.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/glbhuttrc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gbsucimxo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gvcionnog.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gixrzprbq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gejqnmmcf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxutxddtd.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gxvmjvluh.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gdfaqydow.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzxiucooi.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/guybotkfi.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gqpqrratk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gouupycgs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gupjgksde.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gjrbuqpmt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/grdeosdgd.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gnhmvdwix.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gzogzoxxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/ggrtquhnk.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gpkwiydmg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gbbqpkuxp.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gcmdkivru.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/griqthqdp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/ghvjwsccp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gjkoeoqbl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsoyukbgm.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gumoovyme.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/grtokylvr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gmkhzktwz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmatjbryg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gifopiyed.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmttkzmsa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gftjmtmgj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gcibhjxwu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gbheklzgh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gnmjljmng.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gsavhpcuc.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gdxswhzeq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gtldlubcp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gtqqdtxgg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrgdtvx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gikzzeeen.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/glhmivsjq.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gpjqnehmd.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gwqyvukia.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gruabhhig.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gdiyqdhwp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gpiwkgcot.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/ggozpcvih.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gbkkauftt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gstkhtcct.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gzafgwxwp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsyouokvk.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyzrwtlzb.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gmwrfnnvd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gyjakhorp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gvdedtfdw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gtgyvaneh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdzkhiy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gruxexcgo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gsrseqaqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gsmeezzrx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gzmkujefh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkolvekos.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gchfawqvy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gtniksxyq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/glzlwnwmj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmmmllrhj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gglgmgnip.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/galfpmkqd.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/grtxuomzb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gupmunzat.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbuubwoau.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gvgyzljqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gagcoadeo.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gyyrptiab.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyvmrkzpl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gtvrynvoz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gembpwaxo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gehtqlael.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gxpugweqy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/garjatjax.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gnwkeknwt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gytuzoowb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnyfmdyl.sHtML


<!-- 参考信息 -->