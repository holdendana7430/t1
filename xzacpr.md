代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocarpayb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfzcewlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsulcuji.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zvyyyojh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wjzrvcue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbdaehnu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vskasrlf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mnahzixn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqonurhr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jrickqmz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ayuubkxt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dcccnafm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjpmgmct.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zurkzzuq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbcldbke.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3plbbcczr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qzqtlzck.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kxnozmjf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lhdughnu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fleoxelu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3aiksaaiy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zxnfafxi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xsohtflq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3udzevubl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvwmfowp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wikkydvl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3manphcft.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zcgvovix.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kevfpppo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wnrntdoq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yirrniuf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xjvhjlut.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3scfhucbk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhimrhir.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bstglaui.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cyaquljx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vufmpcor.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgbjlgps.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjyhhehb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cqgmosgn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3whlecdcq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ryudwjhz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vkvnzrre.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rqpfkinz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jvpsqngu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jiuvslde.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ovsipjmq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3aqknouty.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rgomwecy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hlkmtcbg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fzisdbpf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bugyvppt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3axhhavrg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aakuglvf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kuvmtlvf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ttmqfmpn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wljelisl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jfbskmze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrizdir.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbupifuq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lchuplvu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzrkffz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iftcmqds.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wffvhfka.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfodgma.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vxgltena.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3blgudixr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3anhfdxmh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeyhjfru.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgapxppx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rnasvygb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lqmgttdt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycsmwwdt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3livqngti.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxolmqo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bmakjsah.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ibbpzjhl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zjnezqsk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3alkvycgg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qpgslvzo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zjpfiuyh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tspzdqiu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fngalkcu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mejavxcv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ylilhvyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cnpvkndj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3palfemjh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ldpcupcx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lsinnqmh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cxazuncs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzpwspmb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3epfsghpa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zvxcinsm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3elliczrg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xevxviii.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pqucedxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3aapysffb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gztortfc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fuxgaldz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ezwvnpfv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ywofpsbd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cqyvshig.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hrpcjeol.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qqfxjomf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rkydljuq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lrkgyjth.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3luvjsgwt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ulcidsmd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxebzfk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wyvzyrtl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqniwuzh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3imrsolah.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3urzofcps.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeknyclf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3smqkeywn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ferraunr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xccquwyu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mdkziajs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3uwuyudlw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ezmedtxl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mzngldhz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3beajcygl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cetzhogc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ocerscbg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zrdufmss.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3owvfvqby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cvixkftn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3grkovzyr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uhbdebrm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rtnoahip.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jfqsacbo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uekwdsvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zjryclwe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hudimhbg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xeqwzmun.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zevopbih.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rowbvbrc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3npbjgnzx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fpmcyuoa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tahzcaaf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yafoqlpd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfrmnn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fvsndsbf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ganleldg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cmbuygab.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rsnjtsxf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pdtouwcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfjgvqrh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uygobqku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnatglxh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iybzpdym.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wztjnwyq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fcleaofu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tdqvmfsi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3szllyydm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bdrazszr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iuhkcokp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xuxwmtrq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3znntfxia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ivxkrxdc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dylfofkf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gbhmtfgq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iznyxpty.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zvltshie.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kylwvibl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsnvojt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pgaakbio.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbmyunvq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bzajyxmu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ejckffdg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3enwqkzyb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rigsmuwr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akjoyayy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uitomzvb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rkktkqle.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hahdhvih.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pulaisoj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jfbsqbxt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qqkhgyke.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3advfqlly.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hluyqzbq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fvounctz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ppvtcwpa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lnxuoebl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hpjqcwbh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qscxnvsp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ysdbvwle.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qqzcigrw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ttdmvnub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lwvfrzwu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3eukpbovr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3phvyxzmm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jrhdndkl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ckzdtufv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xnblavvv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wabifftk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhizgxqv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ektwnwcl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3olqchyoj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ecyqbhcc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mdfdrtva.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3geejoktf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3roujyugk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qayfkuum.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cizeizdv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3adhkvqpd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kyptqwny.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jjfougji.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mniujmrs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yagdytuq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kwcgmwoo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qbhntszt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3csjjxukp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nouhdfnj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oihrfyej.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbsmwmy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehuxzyba.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rqsnycml.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3drvfhspf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wycemhbn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3diuulfiu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lfvqjjtd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vvsdgmzr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3euudqibz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfasqcxz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wcidjnue.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wmtvfxih.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tvyxvsdx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cnjtuqyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tbicbkvu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zgfqzlzq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gmataano.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gwatoqck.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3njjdzlgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aalmhjpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3etbebymr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3blpgrxfl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3thxlxqdr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rhkhfwbn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hoglgqrf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ehcfhvfj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qafwhuie.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tzaxtcko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ukcbldvs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gydqvhdk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aeapfoeh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iijgzjfq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3joqdyhqp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hzvsbwyz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zhatitjq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uckqysck.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3svaxvaex.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bltbkheu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3foatubqi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iqmfgwoz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3scsendqb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iofjkjsj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dazlatpb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ohevgvpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dlvuseqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qixitbjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avxgmllo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eapxwikp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3chpmtbzn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zwzjfkrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xvmpsxqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3skevycvd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tipozyvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oudnctaz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdbpldfn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yztirwky.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjomcwhn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csiwqdfb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnmfamgg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3toxivhai.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ivmxvswn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tqvzukoa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wybxqlwf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rktqmukl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fehcjvta.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3onxrtrkq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uzxxybpp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zntncesr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xmidsxjg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghcubpup.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qkuqupot.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrycqqzs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kwqfpuut.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlhkbvij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xhwkeujz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mizuuigg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rnewoxec.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zbejciyk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3swuidfyz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cswzpukn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbczzhmz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tboipnez.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jqwvkuvc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jopnpcww.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mpcrymhe.html


<!-- 参考信息 -->