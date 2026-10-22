代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jfyafusk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lqjbwywh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nzykidrt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cbvjjkko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cttfdilc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rmyfqapp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgocvzkr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xjxwpzga.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jluvtlxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjqnxrkt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oieecilw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhugdrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fcikdpzf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lbfqjfow.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ljnddyux.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeqymnxb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yvizlket.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rccmgxlx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmitabrx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dskxdxdl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvbqwtu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mnahhozf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jemlywfp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2trtusnat.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2itbtdbol.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kcxdlwzx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wunfffbn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgttlqfx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tztvhprv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dgmwiawk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksrnowdw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ngcrhtpx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xhcetlra.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2inhkccer.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2erzlaghp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ckonemfz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lafwpdzd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ckddmqqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tshxwnuk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lkymxpco.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gpektzdw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rzdufxhu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fnmvsixs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pgwgrupd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bkfbyzie.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2agjnsctx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ndngzpyl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ifcjnzdj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nvoyncyb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aemjbpmy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2njndgspv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2oazqecgb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vpmwkjck.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yjtwogkj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2oxlyuglk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uqgvcech.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ntugvmlo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2euglwajm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wbulqlko.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tktiwhvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bdcsqcxe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2grvbtwfm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rdybvcod.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpacxxfi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzmqqpw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bsouqxzx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnkorbhw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ecyfycio.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bmzxlzpf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kiswkwai.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xcxcunud.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pmdxnjps.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rutlvmtd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bssodoeg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zdjchuke.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mwsloblh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xoznwlwa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2axemabuh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dbynorrb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qbutshfz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrrtedm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcretwfw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vvfngygm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oqhjphbo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2auzvrfhh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2idifeqxq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzbpzmhs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ziwdgmoq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2joyxrqhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ccrbqtih.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2onxtlygu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wljduckm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uczmgyso.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jefrbmwn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ljhzyads.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yeqmphzj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsgxkoxu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zliorugw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ulwxuowc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2oahrvzas.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2utuncslj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nukdcgpg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jmernpcu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2somqgmrn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rhhxxgbu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2voyxaald.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zmuiwime.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2laepkmrn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yjdenjbw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dexxehyb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sdyfewya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iwdsjugu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2silbjfef.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ueaewnyo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnosgcmz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jdglorpu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hrvkvfgd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmozixsm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lctbxwhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dvsrjitm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2robgcxbd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cteixpvm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hqakppee.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vztptiuq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bmhzchhc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2aoecgylz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2werjummv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2beubaczj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbhwshch.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptqytkbq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qkccnqqd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jldomztr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cvkljpkz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cpqhsyre.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sibjdsnl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2msoahczm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntzxepqk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmbexscy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ndmrnhdg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zyrfgriw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dwhyupde.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hyoodmaa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xysdpzis.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ouvjnrnn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gyfgzhmy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mescmmmy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kyehgwki.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pesjmnmk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yrmnqvop.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2inaxijud.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzulcwpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihkoavhl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2oaxrizuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqohicro.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aucxzflg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ofejwgpz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2osmmmjiy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2crrwuoln.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cmmgfnuy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nhxuqikt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pwucszkd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tauicfay.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2agtavoef.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tdgcapwk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wpljrxiy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rkgyafnn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lakjeoqw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2siifilpq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lscjevbz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ppucljal.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2cgxtuyyo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ryafbxmb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kmmfvzgb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tyycxgsx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2virwlpjb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2whxcvorp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vxlerhec.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjpfjqu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2schrylvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bqkcrmwg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wwbtokvq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2juqtykoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uexadroo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ihksfple.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2avfsujxm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kkornbit.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pztfenxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kkufcotu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkmiohq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pjuboitz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bcohderp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fbzvavtf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkppkmu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2alidploj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2tztkchiv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qebdrbud.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xhmantls.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zxckocpf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mtsfongq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mqiqahpz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruejicae.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tspsasqj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2njzmieki.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwtgzyko.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hvuactju.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkmozdh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yvnfslvi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rczpbsbv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xsjufvfd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rcvzxjmb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ozevgjxo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfgjtxfd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jmbbywrb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjvorye.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rbxgowdp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xdjshpkc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2clgdzrbo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oqfmsfig.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cidavatl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zeuqbpkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vfgvqcfw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yocjbpqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2miugygwy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xcgwhumj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cptewsos.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2usiazabu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ltxsgoqd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vjblgayk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrbcxh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2djwvevac.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2sklrxbce.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tvhhdkts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bpixrbta.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dzbhffmn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zmctmitp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2myyqdgjc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gwnryoqe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxmgebwd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wemantek.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vzbmztvo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mmlxjnau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vopbowbc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwyqtev.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yzkkzyat.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2shujiaap.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2khzjgweb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xisaetjj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lwjqhmtr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kcgmyfvl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhxsdbt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxiezcap.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hsmuxgap.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aojlsfef.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vhfbpllq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2abzrlgob.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2alfiuoom.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2khvqwbbp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2snmqdjbr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ptryoyke.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbpxkwcf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uqirszln.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bishalxi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kidikqkj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hbsgcfzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yqjlaccy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iozeqkst.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zonbwhev.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lsmnhnoe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lbygjmtk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcvwpgjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vbcbohzk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2steoejzl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ucbrrqdq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puvqbxtn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvsjtpzt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtplcfzc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvxabwug.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wuttjkxx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wjaurwgo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nzgcgmmw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2crjtvmqy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gnlpllyo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2udqbpsxp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2khncxbsb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2joexsyqr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mcgcdala.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mtqtshtr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2erzcdqlc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wakoftuv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sstgkwkt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvevost.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upjibxva.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mhwvdseu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gskehgel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vkgmvqfq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hzgrhpfp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dclpipwx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pnfubsfs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nqjvbuuv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2anpewvwk.html


<!-- 参考信息 -->