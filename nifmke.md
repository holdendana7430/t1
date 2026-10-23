代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3orpvoykh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yzyvxwky.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3evujqjck.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hhkocgjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szklajux.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vuetgdri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdgcooug.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nefnxwsf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lfeqjmcu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fibcxrac.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3htnksvuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnjxdelo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwnaraav.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3itrsikyk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ombcbscf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bwutvzpf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmgpwuhr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xhfzxhwy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sgonphun.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3plpsxzci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bavvtmjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wsfowbhz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3diszwaed.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ezuakied.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3aykuzdmf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qicoidey.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hmesifdk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bucjusoq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wzbvswtx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vgesxpne.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdywifjq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vauuhssy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvzmuj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qgkdcdyv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rrsepsaq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkefselj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wynvkjda.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itqnsnrm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tkhirqaj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hpgqcsqf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjzpzkkh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmkeibw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xhexndxv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mugomatu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dexyjdnd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mjquwgbv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gzxpphve.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zgmblwdc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zwrslqyb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ugpvdqke.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fffagair.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zsqadnna.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lwwerzsd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3teubxifn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vcdskkkj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vjxnwfkz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3enitwdrm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pzhzestf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmwczvu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gxxzylnc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3najjzjeh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dcngyhiv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ubjazdhm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwmviypv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pgtpehpj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ogqlibxh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wjdzgqoj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3matxczkh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bwofzxqb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dtvtjmze.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3khwdvlin.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xjclwgdg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaercpun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lejmyfsl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ashvjnka.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dhdpahda.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovjwvjru.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yqulxnjf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gfwiscsf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3znjkunph.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jpswubjh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fowwsmgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rcpfqmdu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hhcdyori.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3swgumfpa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yiugpyna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkuivmok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwlcpzpb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3khulwrxi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fuezfsoq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fwnwrxep.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nxemlksx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cskdnelo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jmfvekpc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yfvtexlq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ztcfzmai.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sfqkfiax.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jzifcsab.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3riqovzpo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3npfsmqdr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lsuaptjp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wfsrngrv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yrydsmac.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ubpoigkg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vpmijdxf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sabjneog.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pjpnozkv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pngiwpfa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lqdyxtyz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hpqetzok.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iiildcqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kmtdftch.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3itrflhsu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3knrxhapc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfqjittl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3murhcocr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pxmqjxnl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxqzrkyh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bdwuebep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3obzstrmh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ryrvxlpv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vncwgadl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mxabkaim.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3etqjodtm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzrcgrpr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lonfzdgs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pzsnvqwc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ytewtotm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pdarztcs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzwfdtl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xegplyta.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lqopnmef.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qptfdetc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3shrgqnht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ricxebik.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3djasjyaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fauldbqx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgnehdei.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lerxcmrt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uiuwugkg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qwktzlqe.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mdruztzd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3nibkauvb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3plsjiemc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3msrifeck.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dhibrlpr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vdigpbgd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwtzfoaf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3iwyrdkof.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yoezxusq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bekiepzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnxoelnj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sfmfxwbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knogbzpc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xshcbqmq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3inrrrtdc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3srkgompd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jmwlmelh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3smjqxdiw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rlevtbyp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kuqpmblw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hcarpcsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lddlvvey.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3otywhjtb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kiigbyyy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hcysnxmd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nbadozgu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3drweikmb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jykrnkpy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zdnvhybb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bvplfabv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qkmjqscu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yveeqkoy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3urhufbzf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lrxwdzrz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ktatqnjs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gnkkjdcs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3whjrdsoh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uicyrqml.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uisdoibx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yaspncqi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sruzsfqn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3letzowep.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yfnhmhbz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ijmyuipp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wfranblm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cknawmvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sdqyzbao.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3infztudi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wpenyvkd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cluucsaz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rvmdtbgj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3glomzzxu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cnrhbmcb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3klefmihc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpagkn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wogytxoj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qevnmzqk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nitivdme.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qstducau.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3homtnqbm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlvvovtf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qmjycrhe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3duufrnfy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dopfdnha.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3utpltfqa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nqdnbilm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nshkxnce.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vvxkymkz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dmlkwliz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3obkavhmm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3osfwzrht.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oxlznlch.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jyndfdfv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pefgcfoa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jpvvzszb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkyjyben.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3quafwduj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjsftkb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3iekyvwhu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkqghst.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bvuybawv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ufotdjzx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zxkwlndb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3frhidgil.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymspsmcb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3byxptktv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vuonzbqp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3baqveqtj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3skzwavud.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3epgezeqh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwetqqi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wufjdwfk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qszhdfoc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nsqquigf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bypaeigf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xhfpcwqp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hqigrexj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jgcxtmpd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwcvhyp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tzwyicna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pjeyulva.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgmteut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zrmbwkrc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ggtbnepc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lkrlxdmq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsinhymv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gjtoaqsx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qjurwpvs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lgoslpwc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnabtuyw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rwvgwpyj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dvadklvv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ecuzhznp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mlgitccu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3axasfjtc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3goiidgly.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gzwrzzty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fpecolym.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kxivoiom.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cplihdmi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cojipqxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rdhacirm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qojjjkov.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3elocwmdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kybmgdxd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3frjlajsp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wvvdlbjv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvgsjh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmprigf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kqttpkpx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hdmfqqkm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vpncgqey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3msvxmvqq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgmixzdy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onrfrxli.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qltmmkwm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aixdxboc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cpnfuouz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxuolmvl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kmiqjpfq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bsazxjov.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nujawwsl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xsfwygcn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fgcntpze.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zkpwwtff.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3htutztdc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fhbscfok.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3exckbwum.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dwofxdlu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afgcxbel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulwlmpyq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxrlhvwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jdablvkh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xftwuqml.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nusuynny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tdxkedtn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dzzhaazc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ctdvhmyw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxzxvbgr.html


<!-- 参考信息 -->