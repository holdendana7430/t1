代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ludviooj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mpgrugum.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fcjuigru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jemoaynh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3insmtrza.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fdbabkqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pkbnnggl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dgsonozx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slvmomrq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zrlkbljy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vaknnhsh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3smgbntfp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kiggtetg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixawprjj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3amfyqitm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hoagusvy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxcvixrv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fbitmpjc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jcmuukzg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ocnlulha.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zyarnrjv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xteagkif.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvqcmznz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jdetdpoc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fqtdtfdn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuhqkhhq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dxifdpkv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3llcxhwwh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3avrfzmxg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bseugpyg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eysqlylk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kbscluji.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pnkuqxvi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nembtbmd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hlaipkog.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kbketvzu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vxarelqb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tlxmgvyg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dooycjaf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ufmeoipo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hcfdtuav.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ezgpbvcu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qiwoctfe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fxzsyifr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmycocpd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wenzhcpj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wocvgrwd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3djbabnwk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cpywcmto.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ewzytbmo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ftmcvxwj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyuzesgk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tjwlaibf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uvgdksqq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjngeiug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jdnwhywl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hqesmqfn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vikwthcf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hbffchun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hqmrhmdf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hrdkhbnn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3snzwvwml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkazybk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kztzzswz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xjwhnnme.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qwjelftz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gfazmvrv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3iyibjjvf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdxoray.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3durjsoyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nliezumk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wzxqgubx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwixnvza.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmmjume.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exyleugr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkdmewon.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psepbrie.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zqmrtbxd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vhvtzmfh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nnyrbgyn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xuvzzldd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ythikfjy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yiforsyv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lznkgzqh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eboouamv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xfsyelsz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ysehlvvd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yieswwvn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gtkdxcpb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tbummlig.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pclmzsej.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rhrkhvdq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3obpgcria.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3itcnhkns.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gkytuhkj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xcoijlou.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fcryweid.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xqiytqpd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cxjzsqxj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pozujduw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vlffegro.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ukemnqyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eisaoqsk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3woeoriti.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wwhmtmrk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ovrtxtcw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rghmkubm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gftgutda.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gigjvqmi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yuprejut.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ywmbywob.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3htgmcfif.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gnpttudy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tfrgfekr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yjpsrbaz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gqvlnfnn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqnmhln.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpcliyjo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tcdyuayh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rkwjzoyl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lhhztxbi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3imbmevfy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3chfkylkf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3opdatmoj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmtebsvs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grwxrsrj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dvmsjboa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wuqmoumj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jyraacnk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mwrlmoyt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ncdtritj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xhfvsryf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wdbowqdj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tlxbgvnt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tnpfsxdr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crpxtvbr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mlgzhity.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sycbvppz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxkjglik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxkyideg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mgtjaiyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyhbugvu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hkldzzra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mrqwwuvs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3efcuxkgf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zlkxizzr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fthjysxo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ivexvfdg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cqtmblvd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bibdwuif.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3aotilocv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bugqmqxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jumzqxfi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxjmsp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwevrgo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kwukisoe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dfxnnclt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3btzbxned.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vttkuycx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ysoesbsl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymilwmey.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnvowuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bplkwbmp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dkbhfrqd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ztildhma.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxfdhxff.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gjjxwuut.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dcgdgbtv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elhhwiio.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jvhwkkht.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ohgwsujs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zdmcwouc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3njwfksma.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3lkneuinv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3sjzhkdxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3odgospmk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmrjihip.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubchldfj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3toczencg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uqejsnmg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cexeurcv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3osnafozg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ifpunvmo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jnxiigqf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qfgvtrqt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3imiwiuvn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrshhrg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3syecyloa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjjeexeb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xpcfskiw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wavuzsso.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fjrbzmmm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mnfnqzra.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jfcfsafy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uzvpmuqr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wcfoowwd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynhyftnr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nptrctuz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lyagpcwc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvycxguq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wnwrmemf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3amtbtgkb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3epaszgze.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uwtcqkni.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bumdclgj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mnqofpnp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjesufxs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hsozcupw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kxamvljs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lbrpuxgx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3upyvbgbe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ujfnfhjj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gwoujymn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqnkbnep.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mpyxmrhw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3klbfwyrp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ulflrism.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mtejliwg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hrlmftky.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zulifhye.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcglrqk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fulrljco.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sncjhbey.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iuicyjyu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3glllbwni.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nukhfttk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mzllzytg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pazsagzq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3uhoctiwa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uqmxjfrk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ynanempz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nmveobtf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ewqunsmd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yfesjvob.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3irdfgdoo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xlizzpjh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3thsottwn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3imjnhzwo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3aqcfwwpc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uimtlkxi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jrlknlqx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ifnwnkun.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bhlhmeki.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3khagkmpg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rxtwavxn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kiagmdmr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bamdtebp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orvrguta.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3enxhluly.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zmufndgk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3obzvgnpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rmswrjah.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kmcbiwte.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3caademeh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrwdoob.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3setourle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mbffhsli.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdttroji.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3casuynxn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xapyyorp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mbuvvfds.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfyjudxu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vfujejxn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqmcyou.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xynavivd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxwmtqhh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lbgjaptd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwzekjul.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dokvntes.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3usyokzts.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajarcriu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cctjmlac.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vshlvtrp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jsqgxjsr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gwmwzqub.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nfygecvi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhumvtlp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pscwcodc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eudispkf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbsbabzx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwwfcmxy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zmiksqhm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cgeviypn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uxqyytnb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bxnzhzux.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3iggypmhv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hesmcgef.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjrdnbpq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lngyrmit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bvhryqtc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydgthgco.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3blcrkwot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrcqwbe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3oxxigegi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ukglfczo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3folpwhmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ehdcgrym.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ximryfsj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpvzqub.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zhiuojnn.html


<!-- 参考信息 -->