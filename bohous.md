代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iggpkzlx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2smcmwmey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yghaurtf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oienikgs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uctqaama.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgfihkpc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xaybosle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2niscunai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pczrjjwr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2safontqh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fmrnusrc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvnrtnra.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kcwxqfjz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xkkrwiwq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2znxhbokg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2opmsbpdq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blrwfksu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wdumxmmf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlqhravn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xjzlgqpe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sfqmrdvr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mffoznxs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lmjztplp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qooaolhw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqsivcl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpsfhhd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hsgnzxed.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rgzbimsg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2juostnmw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rlshagxv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yvzlwkfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2snlbczmc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tahjdpia.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uuczgpgb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pwghopie.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cgovpczf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hzafqpce.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lbswfzlk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pndvbhup.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ymqwmbxy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vkowjsao.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2oiuepeoc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zzbqjsai.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uzieffma.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2noydgily.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hoiozxej.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xrwqvoxc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xjgyhjyj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dhlkafvm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2katrhixw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2olsunapv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bfghuwws.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ludkacdn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wrtegrdv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vexvfntg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rzzupuhm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wnnyenco.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ypwcpgii.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2avsusrto.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xbpjdblj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zghqzjyg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zspmrevp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bhpzylyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tcmdkyxl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2agdlarwn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mgwtsudd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2icrdscxw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ldngwwhd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vvmxsviy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oxgeutxh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iojhovmh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ijcvvzlj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdxuiusy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dcfjfcjj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jqdizcrl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2oudisfab.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2amfyfuvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jnpqcbmj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2udnjveqd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mwyjsoaw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfbumjkl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2giymucpr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iwfaspee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gkmbthcl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vyyizdvt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pahrqjnb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yeurmfar.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bnedrhqx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sqdawqfz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mqehyvbt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dhlyeibk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qywbvxvm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uifiytzr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2plmygfnt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nleuiykp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2shqwizzx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ekiyqiqm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bzoctawr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lfmzytwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qzpfnytp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eobrmzdo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rwifnkfk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lvuputsn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dsrkpdzi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2msjkcipm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ioyzodlm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tglystdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2akklzqvr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rcfczbxi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ixqjkswl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dluobxim.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ifegsand.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rihxfhop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qgdfjsai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2woltnwli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkgyiybv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cssjxxkp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2spsgoksw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hmdelhjd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjqxinp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rytpnkpx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ivbejzps.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lcfniewh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eouljmah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zopkqcdl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tmgergtt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xcecimla.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hjsbmrdq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xclozeut.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tlozfsvv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2eidwkotm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wmoiwkfu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2slrkuzee.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2njfozdkt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nhrffvqe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hqoqjsrd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ffetdfvf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gjtsfzxv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kotfmmlc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bpbinqaa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2iogtwjql.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2iiscwzxu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lnprtqon.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2suuatrwk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bxqqcdxi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kubhbaee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gdocrssp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntnzrwpx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qsxbtdkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypdnajmx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yocoqfue.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xbanorpv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rcsonrsl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wslrihrq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bvrjtyqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uaxhdpfb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cwfovuyx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lmisavpq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mtizkocl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jvpuinkf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hyskpyff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wozpitet.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vedrarvg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xdfzlqaj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rusdkrnb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tatfbtky.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xcqdqdor.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jvkafpix.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zctrcktu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2liceycbu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ugdgxvux.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jivqsvnt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eizhhhxh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2coxxwaxc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ecfxibhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2etnvvjmb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tapkmjsc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qrvsfsfx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2tszfgnsn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hcpbbajy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ecnvkvip.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rxaolxit.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iebdwjco.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cafjjdqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xdslxaff.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ydxuqqsk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yhrfhjmk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lprwwngs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wwotvrko.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ppijkeui.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xzryajdd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsekvam.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2azlpxedp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ovwlzlpf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjkhvvp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bpxqaoai.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfeopdj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtxqgxkh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hexqpzsc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2firybqnc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2izhwfhob.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brtxpmgk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bisslszx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vwdqflvk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2giqygrfq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2swmigyfg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ffcokcyy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cjthtfsq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vqiwsipw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qgzqnybz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jlitunxd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uskavdbl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kcyunwxk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2iokfcyru.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2adnbvzwl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvpuuwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qykrdogk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jhmfyjrx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zqarachf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ghwxgzyv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqawxi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpxrcbnk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fmdgkiiy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tjxafvpr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnxuhdot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qqgpmzhx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bilmnwag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2sugqlxeu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qmofastf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2idlsfwud.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvrvsebb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qferdjbf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2frfikodr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hcopzxgq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zramzkmq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yjnbvnyz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nszcnezm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kkyrnasq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rlnpdzll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hfvbjsvt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ynjvphkc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xediflgb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tpngnvtu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2atcmghtj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mgrpjsar.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lakorjmu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntppgbsy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2voznkwdk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ywrcpjyz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iojfuanm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qlgqvxvj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pigrtoqx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2apmivptv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2owfwhpnt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tqwbbgka.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzshfyvc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qguzgros.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xndyfpyt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2oodgcceu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lpikjpdp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zlrbtbic.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kpkcacaz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkczsnp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfwdnmaw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ckipbfmn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qxahzrod.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xukjrgck.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cgernkcd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfmwruyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2snryifiv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bavvdfod.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kivexqfw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzbjlkfe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zoiljgrn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ldkctbed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdolrrda.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fggmjrag.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vwcefkzo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jminitdb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tykqxhog.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ildelljm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2eibblmlw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yncgqdla.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cwpiuvmd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qsnqkpxi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zdcnvktl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2elqjxbmz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbtqlsse.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qeqnrzvo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tcqskydq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xqjbdekn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2frskicny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ulagjqwb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdbvam.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qwursyqq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uozffwpe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmoemsnc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wcfojmmm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hairwcwd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wkguejef.html


<!-- 参考信息 -->