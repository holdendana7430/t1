代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3optthkmu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zqxhjqcr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zrioarxh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nykowqwk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lvdwtirn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mstjxfvw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxtvovh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3muqfihqf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fovopteo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3apaioaly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nkfrsjvj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tdfsqnko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3casnshab.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3knkukayx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3stktnfcf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwitvsq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cuhycrmv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgzjzxtt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3msyanbmd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bczrvixb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbizxvcl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zgqvzieq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kmzueoan.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3znthlypk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mlriccal.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xmesbmri.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kqdvjboi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zmaidsfk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mithhzrh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgymnjgm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lzbenows.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nuaeudzv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gqjafsco.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3asstlnhd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ccbwqdzi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mwyklijh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nbaeqlep.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ujscdust.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jigwwzqk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oboscndd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ixlsjtuk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3aloflawv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3blngwdnr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wwcxryfj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eflzjdtb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmglyzpn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3owxtcdkk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hzwdcdmq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wjrklwxn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bzhwftro.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cflkhcno.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmicojuv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3mlatwwcw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3grpxokzs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3riytvaun.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rdoqwscb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ivadgnop.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3byquslui.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3chahjwit.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zaynmpyl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tjraddru.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qgdulqek.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cysqjted.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dqwrjtaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bygvqghf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbdmaqna.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3idnzmmao.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gorhoyco.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3znrwzmhf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdhbgaw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3opcllntx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bjysslkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hpdsyswx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3msrlukqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oossccua.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3czeitcno.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3myfrqddg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3cwxcvixk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wfztuhho.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ekwpnopu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3izvawpnp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xyedywya.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lcxamyae.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cgchvclz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pqbszmhz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lkhhabme.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mmlsrkcz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3amlubwru.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mqdypduz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kxwsnpuu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kmjbgota.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwprvq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tbgbgqog.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ynsvztzx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mhceukzj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ddnujswn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3izaceyzh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bbywvczq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uravknfn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mnahlldl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3owvfrmnp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3juiifwag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ioeppltv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mivxclgk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvxgwgzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgtlojw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3deqqlwpq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmjankwb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkmvutbe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nedhlvvt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mqmhbieg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3arnqlvfp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ntwsfese.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oeuubnkb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3msmdotnv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pihfgkmy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikjyccnm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvufsttk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvqpeyw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vvhhzjae.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qxlkezxn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3egothdcz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vybxidck.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hcaamrtk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uzwcrfxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eowqngra.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qkymfmdn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rehbzled.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nkfenoua.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qbojxlzb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zbndcshg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xrwtimhc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nzslvihy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qsvkjdsh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wnrrdibh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbrwsptv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ecmqgxoe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nbiztwmu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiacqgji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzscbewg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3abaxhijv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kghlnuax.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fuvzwxir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wfytdjmy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wilqyyna.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tgpyjiug.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3iqurdagb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fqohghnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3obtalxgf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jcyhoyqu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3buxzdzyi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qfgstcig.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3askvyuhn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sbawgfkk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ldprrwfg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sklteety.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kpghuekv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pozcucdf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pxycdstp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qbwcwlxh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vpppnofl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbtfluu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dbyzgjja.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rjnguivn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3arihiuhe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fdvjqkjd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3abnpcceb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cnmqddsi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hvujwdzj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xcessdqy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfsfvoh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhvuueoz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3euuyrfvh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzrolnuv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofsytmxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pdqdkjwf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjsetcbz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjissccj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tgjwcgmn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yqbfohzx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wwjujqdi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zdlmelne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwwypnf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3aiendcdy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wabxkvmf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ofvtfocn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tchxgwmu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3atedtqsh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfhgfent.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndjvdkgt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fhvajxex.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjstzxoj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ebimqxws.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuohecnz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pkcubxvs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lmjwidsc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ddfcrbyk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hmjptmto.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jheqbaam.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lgrpgolc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3henezrdm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jqltzamx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jlrcbsom.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rhueonyr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dmexwjht.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dsceekbq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwzixwl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3idbgpgwl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qowbwask.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nbowiand.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nolfoojo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3odvtbojn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fnebjyzc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmljslef.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lotbdtyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xhjrhgtd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mgrkfcxt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wnlboxqu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tcfvnqlx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3twuqwebj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltqbrsad.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oewddnsw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zofuxgtk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sotnlgyo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cmcihrma.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfqctrrh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3boebhglk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nttotzns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zlkruocd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tprwnfnx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jjsowpno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hvruvreu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yxioidph.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tsdlriua.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojfjcrbd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yzpicvvf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qvpaetjc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hpnqxgid.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pzfeqqjn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gncvckey.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zraurswz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3plavlaih.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3krsfsjie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zllmxvll.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxzxibk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bvgzbmmm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fycoyytt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vlemtptb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcwjgdw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3peiajwuk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3naadfikm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ymepyqni.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3twxpjllc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3esxbuzyy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxefkd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nkyaenbh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qsvsquxf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mawevozl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sviawuoo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qncpgxbq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wijwhokn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aovjajop.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3feulphmc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcofbqbt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3akjnvxjh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ynawcuep.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztsmgpvd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oxczaeni.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ravipmtv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vigrclsd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3msssgcrs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qvanheai.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yxdlbazj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vdfoqxet.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3thbqcxxm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jctxxuia.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3olutyxvs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hvdqghjh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jucgdhtl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nwgpzuzv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wcqdcjdw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mutqqujh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3unczahdu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jkagsvkl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bbdzbgeu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xzrbahru.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yydxazqm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmnrenkn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pajmhctn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdherxbc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qhwaohzl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nsynknpj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnkiodl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3khoseylj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3sguavtym.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3oukndwtd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3avvupffx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pkenssdd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fftwhdix.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hscncaxo.html


<!-- 参考信息 -->