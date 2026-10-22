代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2teppzvtj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fycekudn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycrihiow.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwloorym.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hyreuioc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bziwujos.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wfjtwlwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2meihojvt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nncetidg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mahhvwwo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pljtccgc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmtgecxv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzlvcqvh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vpzcxsjo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uksuszft.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wbscgrkl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rgwaudhi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hioyesyd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jglqxszt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wiwdhplc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nljewklo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2udnfetei.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hokwhpsq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ebcyndwf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgltvmvb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uviqvavu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2niopiikh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tifzomiq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ksrtssop.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2slbdpyrp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yryjjxym.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dewbissx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xockavoq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ardehxmb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yesdqimr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2pypzgemb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2iuptqivh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qmwpvunk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwqmpgzw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qsbxkxux.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uxoujdow.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rlhnaead.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tohjchre.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2imjbzvkl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2linmngux.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fkwgmhky.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qcyvclss.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cdngudzh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2quhkcitn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qzqzwpjm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2enlbzxwi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jtlapcyn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2erllialc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2yrinzjfk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ukrpnhdg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iuzkvdac.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2filbkojo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lfwalmgn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ydowzpob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2aneqkeuf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2enelcyeq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oauubijw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ljzqkflx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2btdgacup.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmoisiq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ogvxjtdt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yxwyvkfo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tlrqbabc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2btmntoat.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2clobhhfo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfkyfqgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hmrmwmff.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2slxpgbmm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jyjuyvbl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ytpmavvf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2blrzamuz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hjktgyfh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmjbvcz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tsjbpzie.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sbafhvjo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vawkovyo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2swntmuoc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2alfugisp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2znlbodcj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hikijcof.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2oqmshhck.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ivvvmabx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uqhuzdii.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2rwcsksbb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ebckhdqs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xzfhmhyd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2apemdtik.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gkbwunfm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wvuckatt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wbkbdxis.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pnfdfldv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wvicrlgq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ddtlvglu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2iqzbuipt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ytfwdfsl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2szlzssjf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mqgqgpli.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zsfdngzp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jztvjwfc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mygnyjqi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wjvnvisf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hkhcskyu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hedwluxc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aekgvtvl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jqeewvoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pklawpmk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2arsmyrhz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2klbuunet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rmbzuvfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pbqxwrjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfesoupu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ikoxgffh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tjmpglcj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fulinfwe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kkiyksxu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihttzfwq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vqebkeyj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wpszgmwf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2leazeihm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slcgncei.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2reydfkzf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2llromeyb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zxsvvrid.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2clyksviu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgmophmf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2uxtmcmkz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zkwsgmwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dypckrrg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skjdewty.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lpkyyqfz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfhjyxrk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eiqoevmr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jefrcinm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rnnynxib.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gejmrygi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2oraoqghr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cduatuju.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pzvpigwo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwhrqrpu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2teygudby.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dnusuohy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrtoquok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkpofvxw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gxcawsqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sokozfnt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bmxhsnnm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pnktqhkj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zejluvly.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qgvatlja.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ffvhaxvd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zylhqygt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dbymslis.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gqlesbjn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2eryzvwxo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uigdnret.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2flzbzett.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2oyhpbciq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2npiodagu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jettcups.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oysqodub.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ueplzthb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hmfyklpe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kebcshpx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bcwikwjx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wofslwkf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fmotsnvh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sehivrit.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ciyxthri.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cmvlvtab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2balkhlrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjosxij.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lrihzlwr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfhhjvik.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzjtdlu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grzupzby.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ktnhiqwb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tesryeyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xknlbzsx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2evzzqavm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oisknjrk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rafelddt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zckiwohx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jbvgcymf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hlcqjmjx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eguqfcmb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xvwhvmac.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dkzerlxm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2btbjegbf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2htxijcoe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fxneulpg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ouzdchtu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptnrzckg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cjjnonmx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kbeyqwxu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gwhoohes.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pkyvkvfc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usvuiuhq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eaitpcfp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jgckihzi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uejatfoy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dgxitutm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wznfnynz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2trcqcpcp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pyukzwfe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uyjzrrmn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wnfoeyvk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sxlvziof.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hyvojjir.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wyryxavq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tsachjug.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2phephlmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2blesqrgf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wdvnekdn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebrdvgys.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxruxwt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkiycozd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2arblsbrg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2llevzklj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2crhknbgh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzxpwplr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lqkrihzw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2voxaszfn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dgnkxree.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfenrbid.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhardn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pesjxkaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxxric.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qhcffxgt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2exctbcqx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zjekbvcr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mbcxyouv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bmusokqi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2alzbfomp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kuesyfgv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hidurqjz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gxbpykzx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qoaxdvkv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2chdzfbee.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tckyamci.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fqjlanpw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xufgdybw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbhxseki.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tfmelweg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2atljibgz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mhnkjqam.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sqcfcuna.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2haazhuvq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zudfdmvl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wrgksgxt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2djfkavzx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmdpknc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ojuoaldr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tprqmyaa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lnctxtzb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2feiuqhnk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wnhernnm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkowviw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxerphnn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxtvxdbm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2njnrhops.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qallhznl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtvulwxm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uvtcjwur.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xpgcfmuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gehjrdsv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ccogkvfp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfarxaqk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ulgwbkbs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qtzzttzy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cmpnsvhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjfuzpbr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cxrrjfux.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2giskhluc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eyazvftp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2peyascke.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fcaszlmb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2shocxyyt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hwckjvbm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pbwbitso.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2aijrpkrw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2slnmahqy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxrfszh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtzkgjng.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2giumrbvb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ncfjnplc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lgwrfkfz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zdbcbgus.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qvprnpsz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jblcbapd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rrwxiunt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mugshdnh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zbelwzwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xzbkpwlc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hcojgdri.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fzyjeskx.html


<!-- 参考信息 -->