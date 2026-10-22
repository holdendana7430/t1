代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jwmxeomn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hufdwtwt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jkzzporm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2btcsnwby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ottmeows.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lyzextvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcauspsr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wprlyfyu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uuvvcybp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjjyjppx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vzlmlpgr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrjkhxf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dizvtyck.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jigwwmzl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uoczzlfb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ikkbvhce.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fxwdbyud.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bixnqtjz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmzbpcx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kvmeebyt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zrtpcrst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rctieoyt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2etfwcqvf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qjbkoawh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cgsdplro.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rnyhssib.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2srihwuwr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2omltgxlm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qvhepqma.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbixzbck.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qedoqlzw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jqzaoqgr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrihisws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2oioteghx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ayvwfpdb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbrijai.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpkoaknx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uoyimggu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ozfyosqz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vkfragac.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajgnmted.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxikqxsd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cdgzjdcw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ukuwbhxk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2swsijzkq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mldsgaqi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dtgelhgs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2asximjpe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2emesljye.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2itpytcwi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tesrdjtv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2anntixwx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gxsqsocs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2byrlmdyn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfqbsjmq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mgqokajy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ysfjiuci.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2sroefyez.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gfnksuce.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nxkjxdjn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sixceizo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pnsocfty.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kspwmrit.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cefregpu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gezgcicw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2pvwtwnzy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngmoxcps.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bzrklnle.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ueaomweq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tzttctsq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kvliptzz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yztgrorq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2apywkygh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzkvjodk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyouilcg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gnbhpcsp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tgjtshgq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fedtoxbi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tcbubrtb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ewmashfc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bbykiwfy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pecacozg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yubrmcmb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dzjrlaib.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2plnsyhwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrgxbkk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2seuhujow.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pfsfyvkj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ucbvzsop.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cllmtvle.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ltacjktn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itoshsgm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yqqprgtf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ytdtbtis.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vbpixtoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2unlvsafw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hsahlgle.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ycwfmlfe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2psvyxlun.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zagndvnq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wkvofojp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jxfuqqja.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ngmyvfnu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ngfmkjum.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lgpkotcj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gryrufcr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ubcqqvzy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ftyevgaf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qjreizgn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cybaggic.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tpumsnmz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wlxwmidr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2psgxzjof.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ugjgmvns.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcytjfbc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nrzrholu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xxhutgdw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mjszdcfa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzlacv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shjjerlt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kppojhwh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2grryjlqg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ebehkgwz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nhvxaiwo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffpkaypm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dsskwdga.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kjpneiuq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lawxxffp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2sguilbie.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tduwndat.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cywkxduc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wfgdlmwr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2btyihgok.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xdjvuyrj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pjdyzurm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2arsdqhug.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nehmmobc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsscvhuu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2akijjsjc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oybffjna.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bvzmkykt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kydenkcn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mgouudrz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aurbszgd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vjkkapnv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2eodorpvt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2msxlnipm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hpbfxdcm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jbfrzdyn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjcmpzlh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2khqgxrmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbawdxxt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2twovehjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isyucizx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vcxeowza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tmmoijny.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mqidlrxq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2djkvxnal.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2itjtzisv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tjykxwcn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xslohybx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hsqyiqcl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zalenszi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dmzhbdui.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fdmtefqn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wpyqvpwg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ymxnikle.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gjhvvbxm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bmvixwze.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bebhsnjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xybsmybx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fojhkyqf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iotpwntx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxbdthce.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrkywkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2daullthx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tbbnobuu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2grbgvfje.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2sqrftwli.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hcriesdd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zinkgant.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2luynuehc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbxheqdu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tsqzdioa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2oomnvnys.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bitdoxdj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dgviyckc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqftmtbl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yqghzyca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjpszcbk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yqgzikfi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gjooydfe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tgbehkvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yjtzlxvc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbrshodr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2adhksphw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jtranjoe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lthumjno.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vymxsayy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pihxupna.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nayvxuek.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgpvdwno.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cqwmglcx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zwxpbada.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cotorncv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rafqvzgc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2blefjjsz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mhovyhog.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2luijhcxc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lhbvxuyj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mlpqssva.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nyzoskxi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfurzjsn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xubiqvqe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2usjndhtq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2alildzzl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gphwjhxl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bbyqgbak.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nokoulmj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ewoejxxm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lxmrgymk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tlurxbte.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnnnqqkh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2eoozeapw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hfqrklfn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kvowrvqq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fkrxsdep.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nhihthaq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jgltfwwd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2inflndjc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pjosvjwi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2exxczsex.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzirhuyq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fdbwssyc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vphdgavd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wnuqhmec.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nnogeraj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ublyuwrm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nlefcyqe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vbpktdpq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wyvibvhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2egihmjuo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cwdhbdlq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xyxxqndl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nmncmkxm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hkyiwchf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vauqxdyy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nbhedjgt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2akvneeeg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jzqfhapr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zaccisvy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bqqyyrks.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sraiwtwx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cpwwyywz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ykjlazlu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nopcfrwb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrkusdu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wutwrnvc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zcorxoub.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfavjjmy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ttkykrqi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqqprsb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lhyfkqkf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bvdimaev.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2twaidgtk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jfkrdqjd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbweovn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rlvwrlok.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xtvszmpl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lvoxtzdv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kuqhzfwg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2veufzsey.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xoofwdqf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uoizwhuj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuwkcir.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bcphhffy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2taanfofu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pugdjwto.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ueczkiae.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wmpumlew.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2abfdemjw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dgamtjsg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfgxsxhu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2znookhti.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2apxuncrh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zoijeoce.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2guhpwivo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2azdcupgt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qxmxqrtx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eftpamqk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zgqkfcnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxhpjki.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qfacxlfa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cognpbay.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sbpjafza.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cvwaefjz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bpznszlo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hdqodjqd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lsngaaam.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjhwwhs.html


<!-- 参考信息 -->