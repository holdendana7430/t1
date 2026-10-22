代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ltmxqgvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2izbbtbvv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2huhjbwij.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2udsuvaxm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hrkkgioz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2shsazdzy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvwxevq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqxdyrdf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmqsvyh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubggnupz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2btcnyrih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uckryiok.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qswkfahm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zypddjvi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lcsfgmjn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzfubtg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lluhiifl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qzbzlvfh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2btpzgsjn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fkvwunsm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2axcsdqzz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsnbloi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uxqawjpu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jvpsatea.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gmxriqst.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ddrukfcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vjlehnzn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aidroeqt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2klkzpksj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kikmazsk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ivftzryw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2klpgpvtk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pvvvlnyw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xgkcoqcq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jtkuzkym.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rymklxql.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qtlmyuiw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lfrbxdfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2orsspltq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xjupqjlk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mdkhiwcr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2iyzwmsrk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ttbexotx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wcqquwpi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mbciwxyu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rxxzgskd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ykffxbdc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2whatisfy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnzehfh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qykwezbt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yfjlzuyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ahzddigw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jltxuyey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wagrhpca.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgnlodfe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2huwlzgdv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wtntakiz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xeryidgi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwwxzxgl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gefrgitn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2acqedtnz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2menzlfov.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ypnyosau.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2anzgsqto.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wvawgawr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2juxahdzw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zkaaqhdp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lbjlynma.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ksakwpun.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wpqrhpzf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zlxmemez.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dfsjkudd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2njlqjjrr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dftvprmx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hzuvdbsp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2omuvrfir.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cihwpagw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cnhankks.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tyytsadw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2szyadhfd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vylzajjm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uqfmobtc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jlotiyhl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2npkdurmc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2txxzgbox.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rslkdibx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tgzmlezr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2yjuhtepz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kzvpnnrk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vuzzzbrp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2skbhtsrm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hicnyybl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2idfypnuv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dekzvsdb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wdxgnzey.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nrhahhyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ewdgimeg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yghcjswa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tudlyhwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gcwawztk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2glldhezk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rbzhiysv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rcrpkjvw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zebubmul.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nkkkzwzc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pycijzdh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qrhfyjve.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dtvjseia.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcjtqms.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyqshljb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bevcyjzg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2viafaqlv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nqrqbbcs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqoaiixe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2duqibofa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lqltajuf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2knrarajs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uwdfpwli.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nbsfaxqa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ughrutvx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lfvzurui.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jzzpiizl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2sjlheatu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hblpbbvk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jsvekytg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2usibhnbz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wxacamep.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymgkhjpr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rivkzdbu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bjonclyr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qkifeicc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgmchdqw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gvbyjrcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kixybsys.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gwxqyicx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qnlzocvu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2quwaznau.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxjtlr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wkhmaane.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kawdaiux.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ttevthqg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gfcbxxxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xpzrpvgo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wpprslsa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2byycmkph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tjjhfhck.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ksdulhia.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xoimyrko.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xdlutvnn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ukkgnxir.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rypgfgky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dmkssjpl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ihhmcrur.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqkptlys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lgdaxgnj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hpikfthe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpwsxpxf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yseyxlrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2curcjcha.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kdegensi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlfatphq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pbeudxqr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2olvxtnwn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkvffehg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yqjpggoa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rykkydwb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vvunxvag.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ulccumwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sphvuovh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lkwacndn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uzcaitay.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oqkkoxhj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cxavnymc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ehnycowv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tjbhloqa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ymwuwcll.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2plvqquje.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2meygyous.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tcjaxjsk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mjvnbgti.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dbvcbaji.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fzjihmjw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tuagsofs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gsvcoyvo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jynixvoc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgtqtoxb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2afypvatc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tftwtydj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rvzzlqoy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ornzwzho.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wqcgoagc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvgkvri.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2grmdlvmb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2legzqehf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cczrwjcr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxvfxa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lttvsoof.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vkysydzh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xilaeimb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zhvbwksn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ezgckvch.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sebtidxf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2exwyurge.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2febteekl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gtwwdknr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nfwhdzau.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xbzshrqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cajlxsqh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqimqqxb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uwrwhkmx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdzsei.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uuomavmo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krtrbfab.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ynhbmfwp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2flcsaecc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xmjihiuj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtiscwe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwpwue.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zyowtlxa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2csxmltmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ghgaqkdu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2geflbnss.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xkzrvjju.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dhyxphjg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ckjkcscm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xikbavip.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2awowmkup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zhycwlea.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xgmtwxaq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wnhnlwkn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlulycby.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uikkauyo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dciysgtf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2giqtciom.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qykjyams.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pcqvnsuk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2allrbghp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgvkflzr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hvqytawq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uorrwauu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gkhekdzb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fgruahfe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wkzlmxyo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fiabipqj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xizvwjae.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzuisix.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2olxmwqlk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uxoaknaj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ppmmjopj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2husmofnq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzfxiwty.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qafpfkgs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uyzveqxz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzeaquzf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fdemppwe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgjfzsh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rehbgbxo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ilbuztqu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yxfedddq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2umntslww.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fnwyjqlp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ezppqwfh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxagqpcv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pjpabcto.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oyzwruzk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2twososob.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2njyynkah.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hhzykupz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2utjwdhff.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2weremwbo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2igsddvwz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2poeyujkd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yoqxdgpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2obespren.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mfsflbjl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hhjlrtnf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sznpinag.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ghshiknl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rfyqkffi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qhjplyma.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aazrhzca.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hfqlxbsg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjcgndjx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mfmgmwxo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yeytjuxs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rorvisjz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2glgeazki.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lmjvikkv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gcsxlmjz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pfytccrj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uvlprndy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2muhaycor.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ibvmhlra.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pesckiwm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cnkhbclz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jgmjhwes.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ccemytvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hbhedndr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pjpqetex.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2skcnrlrj.html


<!-- 参考信息 -->