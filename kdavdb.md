代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qflrekvg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ikgvdkgr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2usqrzlbr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vynmdoeo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dfivlyod.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wtxeusxr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dyzhjdet.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jcymiioa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpiykawm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uaarzfrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjxhtuzc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxamqihl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2flwsczdf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmkgdgw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hsyrbktt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqypklvt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfpvucyu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ldepyyvi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2eisaomvm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wunafmtt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mcmplhxm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yvofpoof.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qxgfyurn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjtzzjyk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycrkbnlh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tdfmqcse.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wfjxqlka.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ojtzprhf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2stmzazqq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpnkqmti.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ktsfjeek.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nunhsmdn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwwcmlz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2btrawind.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjakvop.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bonqtzbs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdpqtzsn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nhqzthiy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hmbnyayx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lbzotjsr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxqyxjpp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ahoscead.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sjfuvxel.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2igzyjoxd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gkrohxbr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ulpuqiyk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzzjeqw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sqjpgwsn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qvzjkqzx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ybdisiuq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iuibsujd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rxshrmke.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ihogdiev.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2plvrwdjs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2iyftidfp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2khcpqujq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cuzndtld.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tdhfkaet.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ebchzqqb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2outyimbv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mecelefn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oiqrbqpg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vjbeguew.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fdxikmqr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lcmxnoku.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cmdtvfot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2noqmixpy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2njayrege.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rlvxohuz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmcfezp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2btpekytl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2admegubm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xpkpyarv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nplaxsbx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vtwveuuk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2azgfxwae.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofrxeuoe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fssyfhkc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbaxxss.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aadyblyv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wzcxoxgo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mxguuuzl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncqaqake.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkhureae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vomazodv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ggkmbong.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rfqmrpru.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qwvchjxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pxtmtpdg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdfbqej.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wrkxbnup.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fvmfmdwn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2elxrpnsj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ldynkwtk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nmdziysl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2krkvuemu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wjmpbkzp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2glggqswx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yijzgjog.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hbtygczy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgdaivid.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2atkfuzip.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ymxgpidc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rvggafwi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tbteabiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xirpnyni.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2apegiowx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ddzownug.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yrbesxcr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2plfymtsf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gukuyted.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2djqjofsg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2itqgytcy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yioqhbfq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xpggaadm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mmlfyrsi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vhzxopia.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mtrdcmma.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2alrtqdjc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gnkqwwwf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hasxbbke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmuovpcf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2byikaouc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlpfnwim.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qpjvumbr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2msqzobwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2asxlraij.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kotaowob.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwewvazb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2drbigtqa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2chjlfhcc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hjdpgdtl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kzhexekm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2shqorulf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jtbqhdjw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2elxasmtr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gwvdgipr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aluxghmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uxtrvukf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xzttfqvg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tipfxjce.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcebyegk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aywzwfrb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oreupgym.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2grbqwhfg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vmuexirs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uirashse.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lyptcxtc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2swhpldso.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2poiiamjz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jpyravul.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggpnzvrn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nwprwtit.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjuztqns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlbhnuzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pworrhfb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ntxasvhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkglczvj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zhuiwovr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2stiozbmh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ypbpowez.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jvruonms.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2afnyybju.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hrphvwnj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cxnecvdh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2awtntfzx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tkzbgwcc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wzthfndl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ihewpkpl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hkfppval.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sacppywz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xqnktxmk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojiucowg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lymvqrbg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lnguqbia.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zgxhopro.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nzcsszqz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2duraudbk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jyzjdsas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uagmwghb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qberqgjp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldtkryfe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dzeyyasg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fwxdvtjr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ajgmhvld.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqbvebgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mwdlwsdn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbcztsld.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pogtolrz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2litvcsxz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmrilziu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vuytfoup.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gawpaqri.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2enghijbv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2aebafzbs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nrtntvpp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecwcfxcw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rvfqanja.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2riwhrdip.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dvzwafcb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2blvkjaot.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xwtoxllj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wzhfypfv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtyguguw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psmkjhnf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prfeelip.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nmkojvbr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sckxkrqv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yqawayzx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpkemxnz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hiklgylq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mmfcbdhl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ozgcwdho.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zquwpdub.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yaffupze.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hqjcwuwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sedbtnxy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pqggkrtj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jkzavkki.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mlirwutp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwqzlvti.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2eodqzuep.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ptgfkaja.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eajhfspw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hkfswlmr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fopnplai.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qwsrcwlb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2woyskpmb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zkwlocbm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kdiefvpl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zxsjfajx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2enreapbd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hftqqfnk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dhtxvaba.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ocbkffcj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bedrrtnp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sngpjgrf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pibvybvn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eidnjrhm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cgekfhdm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hewyjzsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gksiuxcg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jwvcjslq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qwwuveuy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sniucnam.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yqdbjmcd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rmrwusqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mzthuwam.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tuladprm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pzvtkzhc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmprghex.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jwnjytli.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pntrzavk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kfdvgyta.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kgllfoak.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sjbttuln.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wegxpurd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ibevmfji.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xbszgcgk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ancmlwle.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pftsgxed.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hqsqbttg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hfcsrqed.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2chpqepbb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyghgljm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cwnyzkqj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qihzpcvc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rkhupvcl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxvjucxf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mklvepgn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2amfdhlps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gnltwqrv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wemmneha.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2opguezfv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rrsnmlzy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2muicnuup.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xaoqwplb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjkwwgyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpydobvj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ibiapygy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rmtibzrf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hgvxayqv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rllohguu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2whaghcnl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pqftqpzu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tpufqmeq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lppajrkx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2imnikvbw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2insrbkbv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oexwxurf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zqhwglrk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nzqwqevv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wqiehbzh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2crbhxtox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gztoflqi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jfosinbp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrnfxmtm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2awqzmswu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jmhvnkwx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sojbpnlo.html


<!-- 参考信息 -->