代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyxyfrhz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbpfthz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mmolznok.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlwzakz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nfphewol.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovqiodda.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3emnrujjc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3imdbcwsg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mvyciezq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jikzazpd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rthvuxew.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mbndeujy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fnnrgbbc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3flnimkbj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3boajoxzq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3swhuwulb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3psbyooui.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3amktrsaj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nldqaxwf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bivowpve.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qliwebdt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvdmbub.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kjisrfrn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jlxxpikp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxhdzs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gnyrtvyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvsnnzjk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mzumloqx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mxptxrzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ynuhlcdu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ukalqrqz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qbhplgld.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uxpkcsst.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uwevazsw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iakwvyym.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wymhdmev.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pmxgobqn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fleqsntx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zbodtxek.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lflngqmj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iovlruof.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mxghezsd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yrjnahag.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3oijnivwo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3khaeezhy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdvedbtm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnzirzk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vqedleeo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xehiifhv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyfgupid.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3btcukzdk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3miiktmob.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3psioirvn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bcjpuvib.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vicjaxjj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3akfczdxb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nzgdcgff.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cltpmmiy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3raqujuxw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pkhrqfql.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cyuyfpea.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3btzpouqc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kanqvwzv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ctgwtffj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vyrmfwof.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lpuqpmoz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pvsxvblt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ibuhaapv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bzoazieh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oobudgzs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3avviddem.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lbgbsjmw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ulvinscn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uvbghjwe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aisfqjrw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ykgudghx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ywigwkyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yalevrdo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rlucqbgw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fpowmbkl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hyzsixcu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gymytkpq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3znfjhjgs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmhixtyp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pxyzmwbo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3chiohwdz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mlqebaae.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rlwehsns.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3slchukse.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lgrsldyk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3whzzgdiw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lqlfkjvc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mtiblrfx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmejqjrw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3byewnrpe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mycenujl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jkwqwvnr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fxrkscgj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3otmewxzj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3puzswbhv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aortdfuj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccdrrdhn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3isrnrttu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jeoszlpz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ymdqpmsz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3unwmaxzf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgmsobwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wqufsadn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ncjynmsq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ukrmbqqm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mixlwgkw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ijwjugup.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vwojfqmr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qkorgbat.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3minhsrzz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gjkraxgr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sgmvxtjq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3iruvcooc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fcytuzbb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3snwhwiqz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zfmyuyiq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bxsjsnnf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vxaonlvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pcskmolc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jzngbhpv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nicfvqbn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xsmdncda.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bxcpknwk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kxyedfnc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pnaswucs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tqkossiz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jrrtxdeb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bswqefao.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bxcanrrx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xzdijbkl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kdqtfumu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mojstojh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwpicxgo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hbmrinax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3impmyhlm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgivfloe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pglyzzoq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3uprkisad.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3almpkrlm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qzcxeodr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lbcxuilf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hjengxdx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ntymzged.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ahazizea.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wlfhgdrh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wwlcgigf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vptftnzg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cnktphkz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxmajcjb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iqpehhyg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hblryqxy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gabnupab.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fguidvoq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qxioycij.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qhgunbfc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rhmbnvlo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vspbhans.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dgznecqk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tlhcrrxb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3unkxujjn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eapfgute.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jqxfoxlz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jqxglfbg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3udrdtvkd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqndtwzr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yersyzme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bltgjnsw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3spgiqmtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdmrxfdk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nbrpjelr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iposyrrn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ucpsnwzv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hvxdgioj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3llanwsyc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3geooctno.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ugzjdezf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bdperukh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lmklzlxc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3egjdtcbb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cleyokqe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pljylmid.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bcwrmnwn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rlqeocrs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ewxgzkgv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nadreaiy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwxqqnh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iaevmfrv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sizflkxz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhhtggx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgunnq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hgnqspen.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ozruxzvd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hciurelx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvkhbgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3komcmbeu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oplznxwg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cewffuwq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bwffnfzz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjpszjor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pbcpjqqt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3lrimhzeq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxalaex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzveask.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kwaaiakm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3swuencnh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hruauqwa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3trpyuemq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3muenhuqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3plwrhuda.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qcpxptkj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3trlpntwr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zrxhfvra.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3loyynvqw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fpngtvtj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hqjurmoq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3drlcdvtf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eonelvrq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3adszodgc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pjbnhrmt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lokvlnkr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3emclrdse.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cucfbmoj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3enfitboy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3elhlbxpr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ndqwqyji.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alfaymha.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fwkxtwjg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lspuhzfb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oohbzvjy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xteybgvy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jteulmep.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gsakyede.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3abaghpdq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqkoteun.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3babmwlic.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mxcxhmrp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvktkclo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cetmwohh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcnrakn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qiukdcbu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3geedkdeo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dczxhiip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gpundojm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwmrscuv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bxllbzot.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3blclutow.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nkjqhxaj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tldmvwpo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cdzkznlw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bmpifibc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qmpslyxp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxgoxgm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndiwvyci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zgzdbsqx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ttngnvef.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ufkkpsyo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3soggkuyd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ljiseihh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3geuoigko.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mnguaxgw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3azzdmiqx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3itnxpwiz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hfkoytgu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qcmlfjci.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pipfzrho.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3boexihro.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ghavmrkw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hgivazvz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gqqycyau.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ixowptue.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vsqjxeld.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhuxzui.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwyylht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vjjoaobv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjmgwkt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uzckwacj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3azazwhvn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uixhbrpk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3parcnril.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ojiurezt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhpyyer.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oltyubsa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ngjkbvbp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mvcixxaq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpapzmz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yyqwidsn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wirvdzhd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xyplozul.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvnbbtpi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byrkhqck.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bapelkwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwdhbsoz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkeyagoi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzujvxxs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmrurufy.html


<!-- 参考信息 -->