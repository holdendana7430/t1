代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsfansnw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cpfxehon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsxuezyw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jjfynrlr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3eelqzosz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wwyohqcd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sjypcuzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mudxzsnm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lncrspfl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3aycsyygb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mgadxnjc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyigwdt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xyttnbxb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uidbsnvd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxseqsj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnlokbyh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqbiqtwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ukiepqpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pitwbcor.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fgcbsmjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kunwgpnq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnjgnkqm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3mshloxoe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsvbcu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmubxejg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jiutoiam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eibprojf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mklxcxar.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3csofpeqj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pmsalqoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3msmdpegd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kaperkdd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnxfudya.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3elppjlmy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rnqokqik.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3thfgncqq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkknymau.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gtgbnjoi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xalfyvzo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gnxezpho.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yybodqos.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fqjrvvss.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mkrbtkkt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3usxbznal.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vtmxxxrb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3thecmkhj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tzbmrioa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3liukmivx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zqmvjacr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tutiwstm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3woamuwfj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bjxcyueo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yboxukyf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vqdglade.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3welqplrb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wgdwoyvj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ndtsybde.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3roxsprax.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qaqnkydq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ovvvchzc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uydfpsmm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3daulgtwz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qsmzrbhz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wwksysyy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3eanmkmfi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fixkyqzh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3adhxcxhf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gaglkycb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bfkhtuke.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3msuldiep.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3umxrchyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ovpwadjt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbhxfiyf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxppnkik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmfeuls.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gycmaucu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crwswxka.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkiuhnb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3utzotozc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rifygcrp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpgkinx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yztrjteo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmispfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sztymsku.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jxkzxpsz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tsfnzfbr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ykzeromq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3liyezsvt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uqujxhbk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3adzervkx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wexsnnos.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3drfwjqiv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zzmusltn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3piqxezra.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kfdydmxh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eaigjnvu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eqxnbkig.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rliilwzf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yqeduzkx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dgmpjnzu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tewtodiv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wqtauego.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mlhmyruf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3deonolck.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dpfblucm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3klzhmriq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3walpeonz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pvkvanlr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3iaxxqkha.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rsftzbap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbgwspvw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pfdbptrg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3udalucke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3budsfeqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jnhvokyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xotlsrmw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sejyfuoo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hmqltrls.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ycmpifpj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wfdeixkt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulqwvboa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rlvrkaxp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qgenvdfs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nmsfyprf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elslkdjs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cawktcnu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qudiizsv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cminvtuq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3iahmvxjd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkgqnafm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dpkjxszc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yohymgfc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xupcwkeu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dylyhrrm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hcbqcdzj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hvftmrbz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tfaxfvqz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vhxikwyt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vcwilhjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bqikddjt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kbkyiogm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bnvxdxne.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jwvnwsac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vubrzfxf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ipmzixjg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qrlatfhk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbsckpkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdeiyxqu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ebtvmfiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycuqvvwb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3urbzqpql.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3efvohdwu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3epbatfsh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ncnoahef.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aoytrizz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jopmmvca.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3aamtcfji.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lbrqwjey.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dnkzeann.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qjiegcna.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jcarrdny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ovlvejuv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fibnawlo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bqrpwzan.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qamncxhj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mbudkdnn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gxcaeozo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3oneownub.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiaomhbr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xiojjwmm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfwzxzqr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3aqaejmli.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfwzytwz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjxnhngk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uzvdnlcl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jhjamjsh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggktobfl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qbictkbr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pebxerdc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bpcvxfut.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3urtdykff.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3juqvikup.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eoodblgc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jyupogeq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqzobez.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xbueeeco.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jvtprram.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yuddnskt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xfrmetoc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qrdrlfya.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qsbvxyzw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjepphr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ukpsfaku.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hudvvtrr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvyskign.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wxboegcb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ixgajozy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmrxhkbo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3frcirbpz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fmjzjswr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pfnawbgb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drirhzjl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nlpzzohv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ajjufuwr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lihwgkia.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mcrnpuha.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cbcbvjye.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltdkoebj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gsgbiiab.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixcdwebq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lrozfkke.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ovsmpaxo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alaiyxyd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3inusmovk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kpvmixzq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fsnzxyps.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lbumfqez.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jwprylnt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dxlrvjmc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bbovirpm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcpeyfuk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qetbkmqj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wirhsyqy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rpzrkvsr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxudisrp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wcmtzcrs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3evtrqsvr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zifonehc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwoulvxd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cjhxbdbi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fspbdxeb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3geklprfx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cqtlmbhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbohfet.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3frmgroys.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wqrwngqr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zuieiwxj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xifyuyyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3znrhxeuh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bjohopmj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3najqcjdn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lkojfxio.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yuitpbsv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tmriydxk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pctznqpc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cxyqhyma.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtzadzbw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wrnaxgjs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mgxnrifu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fawxyrme.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zokzxgja.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrbpblja.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3czxqifsm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3joapahhl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lnypbngo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hszdmlbl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zqtwffpa.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xqbrdcme.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bysfimud.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hciruvdk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zztphupy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmbzwwq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzwdlwm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqmveovq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3opyaubtc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uglctskf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfdaoojz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dntatvmi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iaxznemd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jaevqkev.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vsihiyuc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbppizlf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ojqfvsmb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ecjqzrvp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3brxkhueo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zovxcqci.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tuupsibe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ulpwvymb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3soxrcmfr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zxpacgsx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jomxilqc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yeosmrpi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3frbfvrcp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oxnjjezs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rxzezyeb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qqhcjqnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3loemfjle.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbuifntg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3piqxrwlg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbnkakz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wffxtokh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ovizvvts.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tqnpdzly.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rgadlgow.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jymsiwsh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3abgztqjr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3huflmesd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3innepnvt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oezpzgzw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iznyuqvc.html


<!-- 参考信息 -->