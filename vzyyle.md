代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dvvhfwtk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xquvzxey.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xdqntais.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmbitbt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nehxoghh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ujlogalc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcmaeypd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtvuntzu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2slyqvabw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nwscunrq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfuqmry.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljkieylk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wonwyrfb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2clihdhlk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vbipomqf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wohanldf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kenjnicl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lniwpykw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sumxdpuw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wndlcsfj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrxxyxrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bvjfjvul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2txjipcxe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2aeapyekp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cmmfiwso.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jmsdacmi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ucktmhzc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2abpziwqt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgrwlccx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuuigkon.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yytedpwr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lnynpcwp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvrbwypf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtibhwsr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzyhovh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pkivjlfl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rnmyfjin.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2oiqiedlv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2madvjgou.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fsmispwc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bbsahxrj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jrhzipip.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xvtlwbzn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2snywsawn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vncxzljw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tgejplzr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lhfwqhhs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yhyltvnx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfefxtep.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vzcwpaeg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qetzpdom.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mnskdfag.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pxrffuvr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dnhdieoo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jidapswh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pclreqoz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2grtshvth.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qejfohro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vrdqiocs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bipzvrvn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qoipntgg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bpkifvkg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wkxguejn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rzzjbkgm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwaempm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2faxdafix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vpgbcdem.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ehmueouj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhwcrtc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qiyisyim.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ziohycbp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jfsigfpw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akmxgfqh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgbilfy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lyafutoa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2huvlcabh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqzhdvg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2enlealqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekizoxdj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhzwhbn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mlivkzrz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qtfycvpb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tlayemwi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dhyugptt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ikdvuqjs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mhrvcmgm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yrivegjs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dunrwlyk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dlilyrco.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mmvhdbkv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xqaosmlu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qjwmhaon.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ielymjuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pnwditfu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yglmguiy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bhizdony.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aemcauii.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jffzkywm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2inujrpjl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jpfrzvrg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2veigzjfy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ibsemocy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ynjsjvoe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qdhseblj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfviau.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gwrllwgl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2udjvtyce.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jwcyfkij.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pcmezhdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wtkoibsv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pfpscrwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yqqalowj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmkunvfq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aafhloue.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zgbftddw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xekzfalw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhdkpqnh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2oagbqtrx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fwxntsjx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dykzmlwe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iykanyeq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2amxuyxml.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2oyrmtskb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aanrjtug.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jwevdyls.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wbbwuxtm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gnrdctgc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2illhiccz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiwfbyuu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ofqvbttc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aogmdupy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fmnqcdrj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qtycskri.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gbdgegwo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bqpzjseh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ngscburv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2krutvgps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sbkfvhlw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wbbxxsng.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmvauowl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vllrivif.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xcfvkhpo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rgyaowao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbjkoupe.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yysfpicy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vygzhnbj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ywopvzav.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tdivlzwk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jatnvmve.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ozmredfw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2csjrdexe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rytjoips.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vbmrvxys.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ikapison.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jiyylvyf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ynqeajrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wnuwyjdl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fkreplqy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2phrxrtyp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2umrosfal.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtrrtyw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gspazwxo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gzpquoyb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ifndmxtw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2plhznhai.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lugtxohu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lchhzgoo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2awtaheyz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcqrxzhe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mihqnmac.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eiprjrii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2unthjxco.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vqpgzaki.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lnrmgljt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lvazhjos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eotdyzlz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dqnkgpsg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ttionarm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jomdnzeb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jlzrabrw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2khkepprj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gaecohap.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2crsaxdzs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dznndvoy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oddhthoz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tghsmmaz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmtlgtm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2muheaaxx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dgpcnzaf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2icugazbh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vokuxbqw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uhdruknx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mkapyqro.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwdiaorp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jxobgwee.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kpojuocs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ygdvqfmn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uokgoopd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nbfyuqaj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wmgrcjky.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2odwvbmzs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pnctacgp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eubtuhiz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vssktfzi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ikcnephb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gbclkadc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yhstgirx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sbeqzpyw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbtgkr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jsadntmd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2spyzihub.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jpivwicq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jxgdbmlz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ntgoovql.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oggdyxcw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2swddbiam.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlxghwgt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2svsqguml.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kweowvho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uesyhhtb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xosooklx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ihiojoiz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xiordoxs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2guxesmky.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xujdnoor.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vjyeidnn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dtfudofa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2whckydhd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2japclljo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qujbjddn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2afnvywsy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2chuthfkm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xufbzvrp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ipjvhyjx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfubprj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ldgstgfj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqgannfj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tjluiyvj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2whemsdbx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wrnqzuhk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tjblirez.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kpaiyfau.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2htelwudv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bvzybzjr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eggoqnsj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kkqjoejq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vlcxtzhd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zuoowimy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdyvxfa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yineecku.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2varqytvc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zkpdpffo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zezounuo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jpevflju.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bqzdouaf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ltvvayqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xhfklofi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gzwauctb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvngbtaw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2irlaotst.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2eambsycv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrcyikjr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dghixdcz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hxcztuyo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vluvgkqo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikbydudh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gevlrafj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2putuxgff.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vnnfpdsg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hucpglzz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjkuaf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vyplcbxd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yzcwzyae.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ajejgqjf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dzeupndx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pscwtmln.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tktpvkzz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jkqhxher.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fezoawnv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zkwjrtkz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2umydtkfy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dpnoxjiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzcrujyl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsalxcks.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2boegcssc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2haveflhv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kxkasaow.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pwxebfge.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2geunpakg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xxmzwqkv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2homhkwxl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ceodntrr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nucjllur.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkwcle.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znrbmwts.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lncovdfy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljmzowqx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fyqvnflw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jclgljbz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kwvemfxu.html


<!-- 参考信息 -->