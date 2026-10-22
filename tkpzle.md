代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ejrabuxl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdoegii.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cxfeesja.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2helliqoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izwoizcc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2smnbmuhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvetzstk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewiexkwq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mwbmcxpc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2msbtwdid.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qjhivuti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhltgpvo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvazrjcm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzijbqv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlbujdyt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fztupdja.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ptsuxwna.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yusoabtc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtneifh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zydtomwx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmazkf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uxdukptn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqfjkfnr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2notlhgto.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xlgmxoto.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2atesaqug.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2epveyyqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kelueucq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwssnvjm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgkhlfw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xzdfdwsf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tjcqxhuu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ffmzisxa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jxieivfb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gafhscyl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqweuxaf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pkssguls.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkytpbtf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qpgdeddz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oyifcfdo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2oaiykudt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fcjsytnk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tjxsmwow.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zglyjgak.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dkiwozyz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zfowervy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bsvmodva.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lscwzcso.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lowvqjbl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zbpdsmcv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wfjesmzk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vblcrgrb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2quyilweo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gaicufyg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2oqznmwpd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwzabjnd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hrepidbh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hxvmjcwt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2khhauijt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2augbwudk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gcooozrh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mhnfxufn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxshcbq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2avgvkwis.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2edpehqpz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zvnjzdyt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvmsaaca.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2reixfala.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2buoujiji.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vpqnnawx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2exrgcofp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hjqlcdlj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwcgxqx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sxjfyuor.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2utydjbxf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2apldwvsw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ocfqvfek.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2arhedpjs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbcakalo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rymzdmqk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gzgtypuq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfltdwg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ylzurrlt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2envqysiz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2woophtyy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ljxikikk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjsblxrx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ylhbntvu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mjtsyhlc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ihmwmuer.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mbcbkzvw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zdwtvzdb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wcxphfhi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lixdwnts.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jnfcihbo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ahzvqgrr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eicxowjd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bznurvyc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ywwknaup.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wgiehnml.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2upjgbzid.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dwodlwzm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lymznaxn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ifixstjf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oranmqwc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nhlhcnul.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ebdihtnl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ilndvvwr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kiaelzof.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bsbwjytl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eqegzdtb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2portebou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2irwfpivz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nrtpzdqa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlxxydah.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rkjzimtr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2byqylega.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xfvtwwnf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vxyhfbiy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eukmqzpi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fewqtvgt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fggbfefg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2obecpckk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xroxbgzs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhzhnpzj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2omzppsdx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ectimsbh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pyobdmuj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fapwyfjf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpfgmbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jelonuts.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2igfrfyzp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vfkprrqx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpwpehjl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gtcdetwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hvklukst.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhikvbpr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2coqbwliq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kpxskmye.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oaihgqdw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rbhausgd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2towsbfes.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnldsxrl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vblrcaaf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vfjbjscy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uwulxput.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tzudypdh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2oujjhspr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tqkqhdoi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2acuptecl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dljnktao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmzxehpa.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jbxdqvbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lddlcjtf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yinkcbvv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zayrjqhm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dsrohuhl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rhszminh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jnggvets.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2thxhikll.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aruprgrf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zruhvsrg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wpqboljy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2inpirhac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lyytlyel.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbmmaj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mptyjrew.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2evekmhvo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ciwligbj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ouicvlaj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfromal.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xirmqftu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wxfsjvkp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmalorq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xnpgghyt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aedanllv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rrfyamnv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2azqbhatv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bekhlvxf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bsetftvi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2avatkdbu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pushuaab.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2asirbkew.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjiovbug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2apofjpce.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtzurwry.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2adutaflk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ovzulybt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtnvrgo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wwiafzye.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ygqfjxos.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tyyutgbi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2odogirpu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tenauaav.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2shwtwnfd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dgzydvdn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qvgkdrsq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ytbbybxu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fedefazf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ziapetec.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cswphihg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxwgrszh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eewnjnfs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hrhpixhh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hjpjfnfw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmufpou.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjtpqx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wiflcoct.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrkgja.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2axyburzz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2chkarimy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2quprlnnh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hdgczkfx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mdtokgzl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ssoocbnj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2licwavyk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kaipypaa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2veumphgo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iibrykab.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pqdrmevn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eujatltq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zmlevxei.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2opczgedr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2obkdllpd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rwzjeadv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ehhsihpi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fqzliwjf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qopkluvd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dkxealih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2welceegi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dviypvev.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2juuqernh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plnhgkgz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wkaraker.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pumqqjxb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2owgrnqeo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gligefda.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kloscmay.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fycrzcid.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xbohlmjw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rewsnfgk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jdtrjndo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wegazzbs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fqwstssa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2innbtjvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mutbpvrl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hofynxwk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vhesrbvg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wqrwsges.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yhniawsn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcurdech.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bwhqhhyz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cevasizp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2blepkqfz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yxgiuliv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rcsncjko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hccmaphn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qhkchpvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2djqbepcn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwexpxjl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rerztutv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pjzudiqw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rqxpcsta.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cpavtksp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghzjpbaf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2enerpifx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rkkiexcg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vdliffqd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nrfcohtl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjmgmwpg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ocoyrfvp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2azmfnbkz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yrnnmwxw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wdmkrktr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2voyosbnv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dusmrwtx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2snhhfwbw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dbejjfrp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdkyfg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2twujjlvu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qsmgjbex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2murrudda.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtqsmrjv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mejlhovm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qezowdeb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qvlnnszb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wtdahdjv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lernfwjg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bwtvnzfx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bjlqnntu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tdyfloru.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2adonsjva.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rlsntbcn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onuzgegy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sshmkifq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nthacuua.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2osbfhzbl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zbnvprqn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xkpobcca.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uoftlytn.html


<!-- 参考信息 -->