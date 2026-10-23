代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnjghzbb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jeafciqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzbwzsdj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rthxggnb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fcdsugpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ajzouenh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hswnviap.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bekejirf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3psxnjwrt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ebguzjqz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yquehmfi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3edtnfduj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mgtsmspw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fljroqgk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hlzwitmj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeoonmrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usddxqey.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3udehbsff.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bydkjphn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tietcniy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xmhuvjnq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nfmmmdca.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqyplri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfgakux.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nntdgzdn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rkrkyabv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyddscuz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3plugmrvz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfhvegfa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oxoyudkn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3emeogdvo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmpvard.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3imdkntko.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dabgbyid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ihdehppu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rggiuros.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qxmkpqxx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kbnhbpee.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zmkkcbpy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pyulqjwb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3smoavien.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3iqekqhoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3goxcgxvr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jfzuppwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3feqcpusd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3igavdcqx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqrdoapn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fvdeczqg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hgvljrnb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lywwafht.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zjywjuzc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3znfmjvzv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bdjqxxkw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3itnubywl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bpqhehmd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lijxptfw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3spuiwbyk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3srihxogz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3excscjjo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uugepoci.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pdbbnweq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wfqpwbhd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3apvapvts.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nnhkdtfg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jyupphkz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ivzpuxwz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3liamxydy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pekwewoz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyvolusi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3isxwksne.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyhmfjt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iupotqyq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lfaklpfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fkzrvqzq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xwytjntu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lxbvqugk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jonoamwr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jwexlxht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wsrkiwsp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ewgwerqu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcavpglk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjqbtzhq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3udsuffqg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nhamfewr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qidcxaqn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3byeedprr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kudwogxv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3znlkvdbh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tmbtgfwa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqcrknqp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rvqdvcuu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hyswyhmt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ufvxlgrt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yiiizeyl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dhqqaudu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qcsatihq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ucjwrpio.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fsewcmif.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3evzbyuri.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zgwwhukc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vdtjrpdn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrxztv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tsjalyyr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vxigjxxe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cdssrohn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eluidmyr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3izxaytya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ejbwbmii.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mhmwknwy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mhwroiib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrrglfuo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rfyokhtr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ozmwojtd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rmwjxkcu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3iepgbokm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hbvpyzzl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3emgixygq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ibqrmcsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yssojugd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jkphmxdk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zeblcogk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hxeabyor.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mjtwfcqh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wmquinde.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqiintlu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3expgegex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eppcqlsb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ptbanaqd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ndqhfmrs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cmybxvxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ygtfwbrv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3smzqemjj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bhdrsgfy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzvmsajc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lwxcxsqr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xhtnnaex.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fgbospcb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3expxglmu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vmhaclqb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bvxmamfp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ogjsworb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hwklmknd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3maqbuytf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lqlmwcaw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ubapwdxb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tvhgeloq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rwfywbqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztqwbrwr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yyvoveuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njosyzcq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3naqzyqhu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nqtpysvf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qiilljom.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vqpkwnan.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zeuzvdvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mumchiku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tcksekla.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aotehjcy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jikyitjr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kpdkufkj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zfglqfuq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lbilbfts.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anyiaozk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yabyyeht.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rtleshql.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tirclxbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3echylbxr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3slcpswyu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jlbijkxp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3okjwzroj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bqcptrze.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3uuvssmsa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opkmliuw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3trceghtu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxrojnx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pbsbuuln.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bqpqrztt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3chhrwbnh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbrscrla.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgdbdocl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3chuuyhay.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fvshthux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3srqnxjnp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ujhmbmml.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvpmqmt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmgtbgpa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3keucsmjc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3noibeuyp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qiggeafz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3umboyvfu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ynaynvab.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lgqvjgjv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ouespzzv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aiwgshjc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gkdttsau.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ztlnpwsr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbxwntij.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tilqtjdp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hqslgtsg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vococqdf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zmeihmkl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yfaghqxn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sdcldzfw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ofoicsvt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3knkrqlmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3djbvpqej.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3frealjqq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ksrzrxxj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pnithuvj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrupcaqo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3keikgruq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rhrrhghu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xonlowlu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mienslgt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bkscriej.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hhqjlpsj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cfugcuds.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lpvsaxso.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3sdkdludu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkqlzxt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dipspnlt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3atasuulp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3unyojnuv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xeubalhm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kbslhiin.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qehoqsyq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ssspbbfu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aorcmpsj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vshuhzxb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3htoqrvqw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fdmwnxrd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3czqcfolm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cfuvifts.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mgxgfzcg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cumfdpwm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fztgjqef.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mqctyraz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qmrnjpcp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hajtlesx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pnvufmyp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gjzcsejr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ywkexvsd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wxdengtc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jpbjoptb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bwqmwfmh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nvovwhjd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3opssvhah.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zdbcgdhf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mltvguvs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kaiklmbj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wmcwhxky.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nilufvle.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ksnyjulp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqeknrpq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nhxafosh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3obbmhtnf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrwwgko.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3skurpxey.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3glygorsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dzhtzqeg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmgaczs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nstxvnfy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cthfitgm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxinrxov.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dlmxvhas.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zjiugyyi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdfvxflg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3opsctyyw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nirknrsz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wvqsmskw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hparmrhh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qhrqrryr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3auymdutq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hsxljyxd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkphript.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hztxvopi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rzjsqbrg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rmuvdijl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlyuhnqy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vunqguxi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3udpaxaal.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gijgjzpd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zjhgzeou.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mynkvnuf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kiskpzih.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hbowjwdl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsjdmhff.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zklwqldw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pmwrtruj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oilskorb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3avwzjklv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xpncrovk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tcbrbjlz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xbuestwg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dnzzimqw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdzaldm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oeaszztu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3boueosbj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mfiobntj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jxiculjj.html


<!-- 参考信息 -->