代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ommghosf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnhcuyxu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdjpnaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pedmfscg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zccsysym.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dvaeiltn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzdeodrc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqbibmq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqsmxpsg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cqjvozty.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dlcmlqck.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uukujrwr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vkgbwnkt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wpvfqpva.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyvtsfzh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2oaghejib.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gsrpafds.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ekncwesc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hivqycnk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2punlmcbf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kvmdykce.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jiyujtkb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rlqhxwfo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ytlpcvek.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tbvaduse.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2dpjkcdbw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iasfmjxn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpmlryd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgymamtd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kepdwwvo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wyfqilvc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xrdffluz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2prjosvpr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpeqszz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zxcilpys.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2svfuxbjo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ondejycx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ircwwhtn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2luhgvsat.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dxusevxv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tthpyqvc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jqaxtczw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2knrltobk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sgxxaenk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wfcbnjjc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2oxbbdkxw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nsqnagqb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oxytjnln.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kgjyqkqg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnlufoel.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qzdxvshb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bzdxorgo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mgngvnzd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qizhbcon.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ljjxzrrw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fjadpcgd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgbqwvf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwiftni.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2imunmysp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tygkgtbz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbjwrtc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dcwqatoi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mteuwftn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pybgusyd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qpvjclnz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iwnmygoh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xozqzgpw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2coggdheb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gltotdnm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hpvqqkem.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2torqjghp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixxuglgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrxbeuq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2icanidue.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jqsrnppy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tqmcheni.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ozmxvghm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2svzqplwj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lipwmgpr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtzoizj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2evamyawq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2oxngucnx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sdfqbemh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bxjaiycd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gubpkiij.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lxmeogoz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ufdheewq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kxvldpnd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xebvucvk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2reodsyya.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bylemggt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zwnngudt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pakosctw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2najdxvxn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2aouerzbw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2obgfqwxz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jmnlzhkm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cbucuzio.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bpneztxu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xmuhrlyv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2juitdabq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yympepux.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jpfxctly.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cbsixuhk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tftzhpwz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2oxgbeshb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aquwmamb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2icbgvgcq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2plnwflff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2suloztmq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gscwvonp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwxwpquu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhsqggpw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ocgfpjck.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nnvyeidf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ojwcxalc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oqstqhqi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2eczwtmdl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xcnzptja.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bympjjba.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2smcrxxke.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nrfhbxrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vnxbzgqf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhaxixhg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yqjajhrn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qsmmgbrf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ysupqsfp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hwmiwjws.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frqilfas.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpnnfkdr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2allxradg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zmsrtkoa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hjubtzed.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2holivtda.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2huiwdusd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zgrcuyun.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qxoeqsyk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lctjqzmp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fwnjhfib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbmtlgue.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tokcxjpm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohbmmkvc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veblxyzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmosivsg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yxgduixl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgmozzvv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lpwniuag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ousrxuwl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zjwbwrgd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uolslwdi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fosilrfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gkknjgod.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2acleajdu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gygnjwhu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dtmmjqdv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zqakcwrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tiyliufi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2quxkmyyj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kysyyupr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlillkrd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tffhlwwf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tkdprxdn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pancahfg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uenugtni.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zaonxunu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjrgxdkq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lxztfgyd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pwnedzfs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qhxnfnns.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zujuskxg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jzdgtidb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2otxetfbr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2akztmhih.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lytfbryg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kzohdxoy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bdahlmvv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2omzfwale.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2naylmrdm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cqhhrvbc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xxhgrciw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hfdlsiva.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ewdqtryd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gexqsibl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mxnjkfjf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wjjhduxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hyezloyf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzovaokh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wexzgtcu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gizadaww.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uxvuylwf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kegwahby.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2unrmzmwg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sasuhhkk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyhlofmn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvsinkyl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zyjvnuvw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2grlkrasa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgyfwop.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sbgvfwcx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qmrvjohu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2evbzmyzk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xyjevfbb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2afazwgsx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fbbnbojv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bsnimdra.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dmdaxtgo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ubztcgnx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hbbwuckk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ytrqkglk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jqzwteig.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ncihwgje.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ahrrodps.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hysosonm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lriuvhkq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmrfdluj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qzmdawjv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmijeqok.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrydtybk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2riysjnzx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lkmuznak.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2txnqssct.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sqgxpdhk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zcsaankb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zeevdpnm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxgispxl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yfbtsggz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qjagxqpv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qmkfbxoj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nbovkdkn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2awfpqqrn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zokqhaqs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xqudxkgo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yhqsnrnb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tqawqnhf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2frfabcnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wjggcknd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lpdmagsb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gsunuono.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzvydguf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2piwezdvr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sbxvgjbi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ujumtlvf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iilfhqii.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cjqgygrf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xdmceezm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2syqihnzj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2smwavojt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sinhecco.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qywztkwa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgirrvt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gidaxqbq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2egkdyzmz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqcgzbo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ofcpsfzt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fdeeecjv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2aunwsugp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rmrmsyjh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gabfupvw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jzazjbar.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pvrbhpzk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2agrxodbi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwhgujor.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aayziabk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gaavuvvz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hydynxgg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hiorahps.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kfacayiw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlxghkqz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgpseaue.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ypqgjbyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ephjerxn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2shuoxmkk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xpnvswiw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fchzvxwu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhojiwlh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tqyeufge.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jyhtjhcn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bfamgmhd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2onyaptan.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tvrbgssz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnitwrzc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nbzenmgd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdzqiln.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2npfrjdni.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rztcwgva.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fokxitgm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2efziazby.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gvadvsvr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2sgurvral.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yztxhzlc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zhnrgmat.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hlympebt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhzobino.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eynjclch.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btqxqggm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vafayatq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jammnuws.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2slqwvklq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tbzanjaj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mwmzsbyd.html


<!-- 参考信息 -->