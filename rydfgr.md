代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uohutmje.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukubftkw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdzaqagc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2flaidpay.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2inivjvhw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ohqdqzcw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgulgfi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrdqyao.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2campvpun.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ijoxphfe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2olgnxgzp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dngcdzbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvrbsuvx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2psknyhkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhghobwl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ferpnnqb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2apecfkjm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjiulbtw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wugothct.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sismymvo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkescykw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ybcsgbkr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2drpzaiqm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgorlso.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2soovukqj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pjsvbbng.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ctcfcksv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vetngxix.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gvndhkol.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zoptrxjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yayrpltu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xzitnyrv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ltblehlx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vdrsacyv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zeosqzlo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2itfoqfmw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qspcibwu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2myrbtjkf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkobknmg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ahtbajaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rslkcewe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2okysqhzv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ccfmtwhs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2amwobiok.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2beeqpbng.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcfhspcg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qbdbrfkx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uicrqykr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxczwxsj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hzvgfcej.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktkivihx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vbuyxgvv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zxlbynth.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dvihpbkn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pitmecpk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2prgxcvfk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pbwkukus.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bidcwmpx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ducudxag.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2yhwgexme.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lkdfcgie.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mcrfcjmn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmnial.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nkwlavxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lixsqylu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iufejlzu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wyvsquav.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yiwhvohp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mqihtyhj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2uxxmvcbr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yyorzvyw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wshbbhap.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2uciiiueu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uingikpf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghcpqpei.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mkkqylxs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmoktqm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sngtflrq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lxvfaaph.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2buvifvjk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofcdbdeq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vrysksvr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdnlito.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ycgmloee.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yhcozkmh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wblrhqrl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tltvxepy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lonmrydv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2npzgtbdo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pbbiyuwk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vugniqif.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jejwfmma.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vesuczcp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nfcjwvab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbrsdapp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hqqnqhbf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rczbgvww.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2evwztjwt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pjjomrdj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bodlxxwx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2msknowtz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2syrqhhof.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jizujlxi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ojjwtnfu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2arthcdpg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qknudusm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xdpdjjge.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bqsdjoxy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hwjoifdj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lvumncsf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hhgnqgyg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wkadokjp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bctdpsve.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ppyurfkh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jkaqywfo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lxizvcwk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eawaxwtv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dhkvqpfd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ldqvbgru.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2shsbjjyw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2icizyjih.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cncadvbe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2krwbhffc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2isyttdje.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ulqpyfiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscybuwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bqgssazf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thxkxfai.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wemfjzkk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nbgumedk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kxcjhtvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cdilxjlo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkazivgo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lnmqjhjl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ncrzapwq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jvbehdsh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2phuptine.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdengzia.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dxjxqehm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iwixwhql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hvpekowa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eeynedhe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2farbyzew.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnmgrqk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfvhwtry.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dizycepa.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2milhmesx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xtezhjre.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sdvlvapf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vsnorsqg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mkxzwwdd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pcjrcots.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2idwznpil.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qjugxauk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rkwfwysr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcecdbbu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rjcwilgc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewaffqsq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2aqoukcpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfanptfi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ncslljpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejwxnlbe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uiuwlbrk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rcnnmsev.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kdosjayk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aaimabfz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2olgzpjeu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nrrifkiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gvddcusx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oafcvduj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nuvcisgv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qccbgoyg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ywhklgxh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2esxqmhis.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gidqnuis.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sfwxkvnh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wibabrdo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeilmiq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oedlpkjo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kyrzwkeq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwrjmhxg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kfictwxs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjrrbt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vvmdbtad.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2obsxfoyf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xtqfnnun.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ltbislds.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jgeiuakz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sngtivqu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vcfllhes.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2halbygak.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yedrxfer.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jjlgvrmq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ejzfosws.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ygtmfbwd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fqffiaeh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thbikyni.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bfdgpnqr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nmvapsld.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fgtjwfqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cpdecjtl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zicwhrdb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ygceqljk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zvekaqol.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hfiznfui.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yodndmvu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kfffuipn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xqiayiwb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qpwyplcu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cavjivrh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bguxacdt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tyufteus.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lcelvyck.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcgsmnlj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rkdcqobr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nbsnjlui.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2veuajizq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ebvwonkz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kzfrjslg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nfxfshey.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kuuctgsc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2srkldphv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cgulqubi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kvgprgqd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqpdsijq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2adgdqsvj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fqkpfftt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vcohnicq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wcqbqjha.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wyluicit.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbsysxfw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2knbncxdc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mwmeouax.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2udwdtoam.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rfdrbxog.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iyqkepyb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fldbmngf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gueusijj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dgfvoouq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hzmbarou.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kgclemgs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ucirjchj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jdflwkpl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qtixmlwz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uokcuacv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogpnlmub.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nsimgdqy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uigsckhd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lgqldqfg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xbvkqfiy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvynkry.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dgpqeitt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ogvupipf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rsjjnibu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khjeswvn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2skerlyir.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2acibvjwu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wueogzvo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tknlppmz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vfpfxntz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aqiqalpn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2huelpkwb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2diicodaq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iolzgmhs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hroblkmp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdeyyitl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2djvmxiig.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nzvkxrem.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kmiwaeyl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqtlctk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fyoljynp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hlcxponl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhnjfrrj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ilcqxcac.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjcyaodc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccbrowbf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2eddexxzm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ibnkdcsz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbquhffo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wxsxmfwt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bvizgnpw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozxkqcyu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qctdqkdu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lessanid.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfomozhs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vwiswwpr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wegxsknm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgneklkf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vnmrcgaf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tepwosya.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zntnslxh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sbcihpgy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ttzgsdcu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wckmcljb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vaptpmqz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vnpsvsrz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ofztfdbh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vgwuqoot.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgygwcqq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2awkyhyoj.html


<!-- 参考信息 -->