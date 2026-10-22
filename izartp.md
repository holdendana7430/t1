代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvazcmfo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vbqonrom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qizqnxky.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yjlqhgux.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2shnvunys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yowdfxqn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gqxkwuxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpqfrwyk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mllimydx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cubgllrd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eprocast.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ycepkdll.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sazgqmif.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qrtqtsqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zlnzglei.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2akjyxlnp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwgfbutd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jvmbsajf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vsdyzjog.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ahikuqav.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nvhwkhuc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2phcvpdgj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ohgvmktv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2afkihsqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2znjuuqow.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2papanwfd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sycckckr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ypewsyxg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ikclxjfi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gojqvsya.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2znqvdcsx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jygdpxda.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ykmdpuqw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nixehxby.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ysfeqrsc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2apihygdu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vhhokznv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2imefpvka.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zxrsgfmw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yyhfldpk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vjbpzynm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nyxdjywh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kujvsdme.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ozynefcv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2efpflfjd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gkdllobu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qlonpzlv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2eegslbil.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sblcgkht.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vxvyacqw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tkjtjzpp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uehkqlut.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lmgkcgei.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2alymbjpg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gzouznhn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2damnwokn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jjiwjjbc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2djcmlnel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ufclhtzv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zogxmetw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2avezrzqi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpjmyoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cczsjhgh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mvyowwvr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2abzirasg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zvehxajo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2btpncplz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hsbbcweh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uawbcdui.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsuemwac.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2faxnfsuk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ihkfvnkp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2utkyfbht.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mppnfrhc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcicthb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2skcwdptq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhcurtrb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2facgdtez.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hjmmjfai.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hkpndnet.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pcicazdq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wyphtotm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2inzsrgli.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lfcqvjnd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zugelpuh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fclgqvru.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xqjdrzcz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rvywqkqe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gusrwzgm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mtiqxbtq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2befyjqvp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kukwssmm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lzbggawi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xebmmxuv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bvmheefo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ukfrkctr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vrvequxy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yriulphf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ymwumkcx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nccdynxo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tqosnrls.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2chdyjisf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2datneccl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jtbanfvf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ycqhunto.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jncbcecp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wjyslrnm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pzifxjee.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jekihkcy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2quzojgnh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xxlgdacu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wxymficp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cfklcout.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2citzysin.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sbmdvryh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gyypjeyk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2muwxwyju.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nvqiekto.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nwqszdoi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xeanltet.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2imitsmws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2glfqohbc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qrnkmgoj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xseqwjru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mndgqtvg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wlyujpbu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkjluyu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bahrbkja.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gsdkxevf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwtjphdv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mjsgepsv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jlysegjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wghxbgkq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovqxojyp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lidkbnip.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jdwkxkat.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qhvfqelv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2boiwksho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2drurjvhu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pusuuvnf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qwmcslip.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yvmxujpj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cigyzaie.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzioqzbd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kkltbwiu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uvqpktlb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mzytfvvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zoenvzsy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nirgwpme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxaxpara.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qhspqgyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nuyyvdqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mcyufbcg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2knzdzjqt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ghffyzqd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iwzywhzk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yyioihug.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wtcgxvxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qwrdscwc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zaisyrts.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2exnapdet.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2igwarudb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bjefhetr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mrpkczfp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xqhyfift.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rciepqjj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uzntaadj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2erliijkt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pqnzxqdu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tauzwuut.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsejgqza.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sysypgtz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cngucmef.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iulmsamw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jnyyecpv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgvkjtu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vbucogpj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aflstfmt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzquxwbh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xnsomzjd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xhgmeidz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2woernocy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rbixvbnf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iyioahos.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uvtxdkvl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xpqoqsmq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jvewuboz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rayyzqtc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pfgzotga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ludmbzhq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2itwwggza.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wbaxgppc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ocwgopwl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uancdmlp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fkodkqop.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qhjallih.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbakthl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2inblqlwk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bujbnzaz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sxxymbce.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bvelosof.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2imgrfhei.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kkvjqfif.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pfjmfghx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tmuydthl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2drkpuack.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrwepxzz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqrvfxjb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2onikpueh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ujldkthf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jxkfxvxk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kcqfcitp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpmjucap.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qmmlootm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ghjsqdyu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2slaoeryh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rkhenbuk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2krslwhmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pkxbueho.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ebmjrbsx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2chfeefnd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cgoaxrkj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lhdvuqta.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bgoxorij.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uiuxkznz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2flafefwz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sygyahlt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bwwxpkdf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2smwpsidy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2atarrjnq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lkxjnrnd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xeesbszl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2opqcvkjj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2csprqgjv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gblzlkzu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nowardbn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hknmplqx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2itddospv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mjlisiti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cmkyhyjp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2niicmmnt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dazlbbbp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykptldqi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtgqop.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lugftruu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mspeqpqb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rblzmguk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xhhgpkar.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2msnuskyl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yxcqkeai.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rfugtuwi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqfxxkpu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwxmbzly.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mcljsokj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2czebpvxw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzdyrypg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpguxdk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ltcbqtiu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xglxtndy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mqhazuhu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzqisesb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2klackxhd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2arsapjkj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gugxdjqh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2znxfkpbj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zqclhuuc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qjqppzjf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hphdkity.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2napgxziu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahurkzgt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jpvzwwzc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xeysspoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vouzlmza.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lebqpuyp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihompsrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xujddbev.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xentdbpf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eydwdzrj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dfzitenk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dmhvsaro.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hycjhmbp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jurlplff.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nkfgfoxh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2woayowva.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqoqouil.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pumcusjk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvbzjgcw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2monrvjve.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ceyzwmbj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywnwxgup.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cnpvkrbj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dhsypcdk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fayaoixz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2otkvvtar.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rhzclttc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilhxuclx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgprqkxa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxteyaw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kkehhbri.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2znnrzjsz.html


<!-- 参考信息 -->