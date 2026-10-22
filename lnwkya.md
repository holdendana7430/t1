代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xnpdzhev.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iadrnfgw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ddyqgmlm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zlmrhoja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2netsnxvh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qsdkxsuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qoalfjci.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxztrkct.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xzspyecn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdtxvlzh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2elkajbxz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aswowzbe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2flmmdxde.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lqgvtjgy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rrkaquob.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qgcjoufg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhmsibej.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zszfycpd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ycdskrxa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oyzmsyag.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kmgtswwf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2agunhzze.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2atlynnpj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qqjlawnf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dxuonfdg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnjbvenz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2flyigdwr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwhlbkd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2owwavlyo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pwipjmdp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjvcxaoi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kjtvgvkv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qfiaqevx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2aqopguhr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yiluiuoc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2igzxtrlq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2avwtisrv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rorfoyua.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kvsuapww.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xnltytjl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2isnsyyve.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2byxerabw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzcujhvx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2aojitfyq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qzsslnda.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nzfrxyhs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jrkfeuse.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qgflebyi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tghkogye.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kwvlqtdm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2phbccjpl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ypthbcuu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ovgpcfdy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tmjtkwtm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2miyheqsy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rezqtdqx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqctjgpz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ifvjqqbk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qtffwotw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ghniwuab.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qwoxfukz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ofzywfzw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2eiqyrlah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqhxohmw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2taepdnrh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnamctm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhjpahtu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rbgiylnx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2grlpfuao.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kjhqmsqu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tbnyufku.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yeizchng.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2esegdltn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnllpceg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gpgiekkz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dmonbhaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pjgfppxy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxpkhksm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2benimhzt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oemsswpt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyhwvyc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yiinmcbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2klvfjxor.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hsglfgpr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tdzrqvtq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hxrbredv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyaeeja.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cknylxbo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gslaidum.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ughjahgx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ngigksib.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xdlnvqjy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yozkfssk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2okgwiymf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kkfuxwmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2megmnjnr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rgjdflmw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pqlsqvec.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vyoxszfx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dydrshrh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xkyjfuxs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kojryshf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cyagsvng.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ehmhwsio.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jasopbwa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tklmxxna.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2sgutkyog.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cjjsimpb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2shwrwojh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ktuispue.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ypkllaeq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2uexplmzr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nmuizqsn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fslnxhie.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aitprgcu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wjwqnuom.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uqpvmtyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqelgxf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jclnnejk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yahevijj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plmzgmpn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2agmhihnw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wcgwwkud.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rzdtlmiy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2umpftitz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vmshkxkj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2retpzicv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zaivbpam.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkyraebg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2crxmsnne.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yrsyewqe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nxoukeya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bkzmsjfu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nscklecx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sbjzukve.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lcravizm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwdecihi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmprgknc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zlsqsmhf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ybxuxkmx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nvtbypyq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hqsgmqsp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pqtvlieb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cnhneals.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xtcpdiaz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sogyhhlf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mprxbctf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xpdqcauy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2apgnklxf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wbpuobrk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2euubjyub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivkqnrxi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wlhtvalx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvoiabze.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pikfeszr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gurxvmux.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2etppyuby.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dnvlstvs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2owruzeqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xlchejnc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xuugzgwq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2udvesxvh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lnwuuwbw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2authbnsy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2whozmyoi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aozbbman.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zvejgsmr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lggkecfw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ugwrohou.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qxgaxath.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bsergdbt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbwqgmyo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2emgiyead.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zqnupexi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gyltpbmk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2diupxaqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dijikbys.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mxkrvjjw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fdqnpcjx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqeferin.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxhugikv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kwicewfv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lyoktpjq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bndvkpll.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2onlyfbra.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mymwtcvq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hijqqmmm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nntecren.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxolhgrp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mbaocife.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxfixctx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kljtdjhk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ikrcdnxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vzmjhhgj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwxnfozv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wakrcfxh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igwxnuac.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wawkzgun.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pkwjbwrq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vditkdpy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uafwdsps.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2shbparkq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tdytugyx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zivfzovn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yzvflwpf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fgpdzrvv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cmfdlrpr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cbmdibzt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lnxfqufy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zekjurtc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2blztnrxp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2shinzfkv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yeavldit.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xpiangxm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lwogqcxn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ltainlpt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oixytjis.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wibaxqbc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcatajwm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hhjzfsyn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ktdsupsg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bqpasucb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qkqzkrcq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2otmvaszk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvamydj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2enknlfng.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qxlqpyqa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mjqtzogx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wngrjona.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2eorfvjyu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lafefxth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2inrfxccj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kljdcpyx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jraxocby.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mplcrazg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kcrgjwgh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kvxybyad.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwxhjohb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2njakzqkw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wkefsmob.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aomutvog.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zyoiwqmi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2htmirwxn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvmber.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jzbwvran.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ewlwzoab.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wcgxtorc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cawwrxkw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2peuejtbh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tvbpphdc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krpayhzv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sysdbbbf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rnmgplhy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bamvzplp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rjsvrvrc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fkuzfbjk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2amivytkn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iehhwsaf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2enrtjqae.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tzqllnpx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntseezuz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fgryygim.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hhqernhh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fvkupuyx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ljyeosrt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tslrrhyq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gwcgsucs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtwyrbxh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2epannmzh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hohcgizq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2grcnfekh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ipfhijxx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2shllocyn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mtrzmifa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2clatfejq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxituvi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bnyhmymm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jtfvzmjh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ubzbbiyi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2daiblarq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2snywrorj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vlajhbth.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2deqfxkmb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yrztsdcr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vgiidleu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2exihnyqp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2egffqkog.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hhcjrekr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvfxuyni.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wtuhkgjn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xufoxxck.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtrxjxdj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oamowgsu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2drgasarp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gxawbrtk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rnptybit.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xcnkvxlh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pqbuspfc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bnoyzbum.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xubgxkak.html


<!-- 参考信息 -->