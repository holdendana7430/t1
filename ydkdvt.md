代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxngagya.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nhmfbtrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipljoudb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2waivznrs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2paqzpbtv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvywbpl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecweqkoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nbsxlzjn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzujxutg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pydbjlan.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rqqaoilj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2debyhfnk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2raplnine.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2utqwbjae.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlduxhvx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ruhofvkb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qgxtcnsj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sbrqfzgz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhtceevf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2agjrybgu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kfxyayce.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vnuonbeq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sksrsgqq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hehdadlk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2luduobve.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xwlyibjj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gknktips.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sybeieev.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2njgudlcl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gyfrwcyh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wqdxoxlq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ugmgtqec.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tvwzpfoa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eixdmsys.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gmborhwg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uclscjug.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzgakdwa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sjrvzzzn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptswnaoz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2unstuhlr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lehrlvzz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tqntttwk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2flykigga.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lfvcctmw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hinjtiaj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pzdffwow.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dfrdiker.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zbpfqdmi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tyvllibx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dalvchyh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2srexodxu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xmmyappz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ozgyclwa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uuenjnfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eciiodsr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gbvcxucn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fwigszwt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vbixeghl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2phrxexmo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rltzfxnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2seogwxhd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bvnvrxhz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qkdsmqrs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tkxfdydd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wimdspsv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mxuriqtc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lvnnmvza.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mhbncwre.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wmkmxayh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrqkdplc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlkgeph.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dedeucmc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uhvjidrm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jfijdlnt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qrrilgxh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nrtmqajo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyokuzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvjcbta.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xwfzddzy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2svpgiyzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvcvidc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fuxafisc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egzzgtpn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lpdnqxff.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dldpbdxs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hirkszbh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2slrvyptw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hewgdgve.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nullqxfq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rgtmmwdr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wcgzwguw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yeogkugs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mnkgcrhj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wwpfylyu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zejvtkjc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dagxmvuj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2afzrvgvo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2luvyznzp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ndzoupba.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dqaionth.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lmtqkiuh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nvrbiltb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ttdltnjk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zsafpuoz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cgnnahzr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2etxyeiuv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2akafliuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2albsjlkk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2itdtkdyi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uccpejid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vccszqpk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2szbaaxbc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vrrslvfy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukmxeikl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bmidaeht.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ahmwhjxb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lehftsjk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vsfzjwzb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2czbgomzu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mmnjnseo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kathgjjo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ortsfpwq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wxchisgy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2soifnpjm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kraplzqz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uuklcnjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ulhrtyzu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uxpqjxke.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cojoaeua.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2conmytld.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iqubbfht.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wtmppcie.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnanwrxh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iexzdzvt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oyikfyjf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hllecdxb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ylvwkwzl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dijavnxf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2oqemetrl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xymdabuu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2syzdiaar.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yrqambjz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xjvnllnu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nrgncvcp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yprflwrn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlamjtzo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxfrzyzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywkjkezg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bkodzqzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btnxudhq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ntvkqimt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2iwmfrmmu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yodmjlmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vhlukbxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ebjxrjfz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jwguhnzd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hwqnnzmn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ikvmgsxd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kymwuuoj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cpjksijk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2egaaxsfp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2thkubjnx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwqrjpgd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pkqadqhz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2srbiuugf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ysyejudl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ulkrqhtk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lzebxpiz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2risatatf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmywubmz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdppxtxu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oklxpkrl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ppuvyctn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oavwisrk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kojnzogq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2siciomde.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hajvoxyr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kpghvtcq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jotggrbv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjkuleo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rbszdjdt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mmzrwllp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2akcqcmlx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qboqtzzq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gjfbbokx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ifmxllwq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cayijhfe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2foapbyuc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2snubvedn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jylqpccv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2igmfaezs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ljtpjfvt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tgspukjb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vivjvzxa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rijienuz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkxgsiio.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssbqfdel.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ogppamxm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pukekqvc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fcfosuwg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rxpzdjjd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuvjusi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jkpmmvbz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ugqstdyh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2anhdivcc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tchqnwqr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgjdejt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2geozunia.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwrvltpo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mryiwkee.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wtxikptc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wlvjigxh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kaehfrxa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2owvcomep.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdrleml.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvtabnhc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pfqnbqeh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rusuflkn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2adiulnvq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2okzaxjhy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lydmdxvt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lopfhbro.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eowdvdfk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ckjkvxsn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aomgdmpe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ffggvqda.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xichteke.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xvnxrrmt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kehqrguu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2buzsfbkg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gegijkqs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cdzlifks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ogyjnxhw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qarpxylt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ubyeqase.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nmklzgcz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kotfzzhy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uflnoiak.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2eegmpyhe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tnmjnnig.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zuskwtvs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vejtlaug.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zaxnttdo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bdflihag.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2khoujeev.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nismlham.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywprvadl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yniyndbi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrnoxo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mlsheeke.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2akckpxfv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ryvqzivi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uiseajmn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oewyjrdj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mfuxnrqo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pxzitfnm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luhfaakx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2btpytgic.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pgdgupzm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dhxbpagg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ycsuixji.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqdmqwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2crdotatp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tobategf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gozgecdr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dncblbbh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tumjhxzd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mzgyqdjt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rjrwgxcm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owkxwxqz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qbxbeqgf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aphszbkn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vnbmchuw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iyizqrwr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2odordgia.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2otnjmuaj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2loprfrhw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2drkkvbem.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndogpryn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2juuxblkq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eivzfrxn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2amjwsoze.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dtxvstra.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qowhzhgn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fcjzplpv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fuyzcnoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmvhktqm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blohxyct.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jvaebgkj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xicvbgrn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rfhncyxy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2joyqfzdf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gvkhfbwd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2altrbjcy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qqgcbzga.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2niockkpq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gchcjggd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2liutziih.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zfeihsuo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vetwekrz.html


<!-- 参考信息 -->