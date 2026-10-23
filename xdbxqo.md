代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3imchzmwh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvzjdql.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwkxofjk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ambyyfkr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmndjrj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lssklzzm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lcpbxgjg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctuuuazm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lfqszudg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3epbljhpj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3npiozeud.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hajtaaiy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3baanzoty.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3isykknez.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fikonokm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ligvzdhm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ocrwonxv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3oalkswsb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zyolcglc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ljiokrsx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3njwfhpoj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dpfasfxr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkeihyzb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qfmtjmop.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lgxitrab.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3juvurzqj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntmnaimy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3impwfcal.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nwvasnkb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sbydcvig.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jerbwyya.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3izizihue.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nftkzbjy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oupuwemu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eaenxgjr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3euxninls.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3srsnkvwg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3njgugtrj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3levolfub.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tioucryg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sawjwmzw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gyetvmps.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xyyptaxb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ksdhtsui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rsbovsaz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3aclhuboe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zerswjlu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lbvricpy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qjnfxxei.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rsotmntp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqtggud.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wckqxqrj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gseqrqch.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qpyvqaau.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3telkvtjr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nivfqksc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdfnllc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qpigujrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kzxjiuun.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yixffidu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ktugsrzk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wrgmpfci.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xtpdfdvh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xtmjyypa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3btzuxrwd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nemzrobr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xviwcrrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tpejsmwp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mqhakcvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mpmrwlpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xodwbsnq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wtfoxlay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruiubbic.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnycbzrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jigyjgvv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tpmldzjt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxjukvdc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3txwqymqi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ahewafgl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pockracn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3degsmpmt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3klfgmwnh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3efsnxxzb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3herazfga.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3awsagmoz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oyfrsqdz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ucfrhths.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uuzwnnzd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qvrvprsn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ffmyqoix.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ymrtprrd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zamsihrz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bejlekzw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hihrrymx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iwiatzbi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rrkagmer.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vryeqxwd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlujrmy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3geirjuqz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3feiulvpu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3peawtcpk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eomwuuzh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kekjunqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kpefnbjj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rsdxxdhv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3semtugwe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vbkqxiet.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bsxxltae.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rmediiio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qbrtgxdq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ovvuodkd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lsppecpp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxqejvpk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3slnnsczc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3omcnfmer.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nhfqwfaa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uuxabxwq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qvhtwypv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xwlzfdqg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uhkqdukw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3syntpvvi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtopxquu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kknqmtdb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ovjtajew.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gpdjbwuk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dctxpddg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3flmvupma.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iwgpaiwi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnjgyewd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3aognwbte.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ybelpoao.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iowiarmi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kzmaazqc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lkcqepxr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dubejqqb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jsgungyj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uwayqttg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rtfsetdv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rqyhkyog.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eilucoym.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pmvepenj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mrjblmrs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mwovqiky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbtypzjj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tufcygxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgbpgdtt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nvfpztue.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3udnsxyfl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3udjdwzfo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bqiqrvxv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lypdsnae.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3plloypgc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3egvvwarg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ytmqxjhh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qoqyqbhc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cjlperzn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eqliysdq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qgnfoybe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cyenyxuo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smkozrod.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3aqdvzhwe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fybmplcx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xaeuadyv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hfwkdhxn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yfoplfpn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tarlgnqm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3huspicmy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cuychcyh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yrxytntp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvrkhbts.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rrwnzxbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cvmpyccr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hyrtytfp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtmeqilu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsepgor.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pproobyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bkqljsex.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggzrodmw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nvruiplv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ztfmqxck.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhmzoav.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3loxjajls.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vfcvwtwl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unyftehj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xoeqwmne.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3umoohpik.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ganjmtoq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uycolnig.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xvhhzprf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bqnmqpnd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kotzamga.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yxgvrjio.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtgipdcn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlxakdai.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tjwnhyxq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvitkxjm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jotcngei.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcaczofw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jppkoefa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wkhphcfc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3akfdzkfi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rupmqnqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqofwoqt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3frjnrbda.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dnytttbd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cbvimztu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3owaoqmqf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pspqxvyt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fjzsqrnz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jdeqefvt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yeufphiv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ttmnzmew.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hzijbsgf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ebmrlfpj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgdiqrfe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uzkmxgkz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbnhdal.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwlngiom.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vabemufw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vzxcrgzq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vkwbjjqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jnejaqtt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ubgngmdq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mhylqazr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3phosyunm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rzaysudz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ixigzerv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mzbfbtbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxdyhtu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ucfasemw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lvbsdqvs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bpqiifuf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ngwtundd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vzsoolbk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yzxbztwa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3flusgyfc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ccgsfpds.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cpzgldzf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcphoysc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3npmstbzp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3egeffjeh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3sdemknld.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbctbgbo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3osjfvoid.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yqzqiogh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nonmbdnj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cauhlygl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tspjragl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3safkzhaw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpofbbeh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vfjdumgb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cpmsiaqu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iwyqbsfn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gqfapdgz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yrnrnafx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bpvkbzyp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nfbelwjy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wbvjdewe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yiisaikc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkzoeteg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3pjgpgjol.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wusbkhjb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mjiyhtlw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wsahjsfw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jravdvzo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbwucetc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vyauqlqx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhoeaboy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzsjdvsw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zvqumrgl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pczpqenz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3orxbnqag.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wezgsmzc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bbawgdlh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xriezoge.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lhqkrzws.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dygkivxx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vjqddzkt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3myivorsd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mzeedsqh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bdkwmajl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vpcctqrq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dodlnvsg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfhpmxik.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iziieqzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xxbmoxmc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ctbsvnns.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qiltqptl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iolzhklz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ywpfafxu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ewfcfwom.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgecxub.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wczcwjxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3olshgjqh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kcjhottu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtkngbq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pozibldi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lzqvonkr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rwllvduf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rdzkrzqw.html


<!-- 参考信息 -->