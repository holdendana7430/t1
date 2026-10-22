代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kwfjwiiw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zmeoapdm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2csamatkc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vwtndukx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2stlyyovh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iebbjjna.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nqdkqpsl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hpomphnm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ctlhtdib.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zwyrcskc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ycglfvtt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jpyqfqec.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mshnickw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjnodlqc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tfakppmw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2svvuogph.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kgjmtyrl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2neruoquv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2djimrcue.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sspwjath.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmaktozt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hlwfbane.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqfulggi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuuxhkwl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oxsrgjsi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuyydcoh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wluqhqmz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdxhrksz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfspinpu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zqrhxdre.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2domkhpal.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvtwuakq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2psoimhfg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hgcghqmw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oisnvbuu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xhexkarf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmxnlyfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mxumunip.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2krrmbexz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vhcbiahf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tthejljc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhrnxhkp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjmzlho.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2snouvcam.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xrvqxety.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2faviaiab.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vezzxadp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fbvukjsx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2oohojwyn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sdzjvnnx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhulnvqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2inbruuos.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2smyqgkib.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxoctukk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bykxhovl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vdwkrgzp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sldopquc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmqnrxy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtduoti.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pndtsjjc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uhapwuso.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ndczzodf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xehppqcb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bmzrodwt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mbbclefm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fdgnvaqs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yfezrdvf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dfuwrbvp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2phuejaro.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pzyxugau.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvqxedfo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gcontnyt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vhrcbful.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iinvnxmt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jcydcyef.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lqyiekzu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ugwrdybh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2roafofky.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hnfbtotg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqnjmhfa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nswxudnc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jaharrrk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zynytesq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nndgrvxh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ppxblufd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uvavihia.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bwxiuxaw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2byrudfje.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zesxtwsa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqlifwym.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ijlxvdjd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vzmqhfnt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pphflfje.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcxxkhco.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2daxhciun.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2eftrybsq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kfdpzbcd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2luzijhem.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rvzoaxjf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ykvhuura.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kgsyqjfj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkazhxyt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2djrujteu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cqryqloy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2shwmtwid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qztibqio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xxliybgd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kgyvhyxn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ahvrajiq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tcmoogxy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zqbrksqh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pcxnvgae.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ieiuvpms.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tnofpurr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2evsjwura.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2odfrdbix.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aebdxksm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lwygsxgj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2llmqdjne.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qfmxcrdv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jnbqjzkl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2utxwkffj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qswkmgvf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cxclcfso.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kqymwrbt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tnuistxx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hvdivuqu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ajjzrkny.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ouuzkent.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ncdqwctd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vqrkhsyk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uklzfkqy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xbpzdcjn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdzblpu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ncrtgmmn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbiylqrq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tzvqlpqh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2suujnljj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhqsqp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2urmaoraq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmvoupnb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gqacjxyw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xaurerra.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2reexifuo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jowjokiv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewhpwnik.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tybyyzhh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oqrkpbrf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2omyfkjbb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ptcloghp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ekdtqpzg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bjzjiuco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmkiqkyk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xxdharha.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pwpfrzsp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wmdbdbxi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mhzlufpi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rmmjejdz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cagtowzf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fwuaoyhm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pxcpiucn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ooykhrkl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cscamics.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrqnvle.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oyujtsim.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2thzkduia.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwpuke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcjcfhcg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nuglsajv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmnfqhqm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahuurqvg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uvxqxbag.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fttfueah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ckhddrds.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2opdcfmzr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dggwngpr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vkekbbmk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ithlpajt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jjtycgzl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tkhmhxpp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hnghbzxm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2amlesmxy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tjmndsbe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ubjksfdc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prvnxasz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ureimwmd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2djswzbuv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcxwqzwd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2onipesyp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ketoeavo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zcebyvud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kvonkykw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akaaqddf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cvbiaznu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rxjunpcs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2weybsaud.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oywomltd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2osukvlva.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2celevkzx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zydojtpq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xydvkcbf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ytrvpgog.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yovcdcru.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ugiklwzy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xdgpvobc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjqhmbxd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dqlfqemw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qdntyeae.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jqfleadn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wxojfzjq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkggrml.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dqxvzawo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2grexctcc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fvgkofvi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2irskvzoe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2crlipujo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrhjqlnf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvdhjmks.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lnuuxpyn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cxhsagos.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jikluivy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iasdxaqg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xhgonbje.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uzgtcrmn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzdrcmuf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hoctotzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ernfmori.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwmulsri.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2logpfvky.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gagrqnku.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2joqdwhoj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ldmtofnz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wosgrijq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hygdhhcj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbrgrpk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yrjyyccc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2icyaxgbr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zhkhxiqs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2csstydut.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dgwyqbuc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pfvqayos.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pfvykfpa.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nrorhxsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qjyfdswi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lrjlxmen.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2iygsedsx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qnkjgjlm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kdghsjnr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eewoclok.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vdumcbck.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nurlixuo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2izzloses.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgdsnvd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mxelkkxh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2urwoxbow.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zmqqmhwt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ufrexdka.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ldoogqja.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cxkipyrb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ejzzcujh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mscfkrrn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kqonmyjy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vivwzsbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gsygzqei.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rmefzjcc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hpivgwgk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bjexlmzp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kkcxgpco.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2egaqoiqe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ravxijzt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eqtzqabr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upyxuzpx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ziovjvxr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ikvzcwax.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uxwbxrtg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mwbvsvem.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ubsnswla.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jkkhmsth.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2eyjpmwyy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2surxiuli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2utfkdzyz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zlwqgqrq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkmcmuw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjqupinu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ooyqtzme.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gasmxnyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uattsmfh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2apnziean.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mftxomfp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wczcweio.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ybciwfdg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eqyzyzop.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tzxdtgvq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2glemtuxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmhupkcv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pcexuzdp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dlctsrmf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vvmmnena.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhtbgttj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rouewgiu.html


<!-- 参考信息 -->