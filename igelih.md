代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hlnhfmwc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2skyjjnea.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2twirelmf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pxgrbymz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mrgwvyft.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wdqdsjzd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ednvarkj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eqjubnam.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gdvjcpai.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zmmayasw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rudnbyuc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wqbmuscj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2teomxxqd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fnyttmxo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jhsrcqev.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kjoweuvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvmvwpsr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uvwszdxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfexnogb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iolzmksr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2canmxase.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hqfjohzz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2spqdfktc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bgmjjjwt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxtnxenu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2itfzspju.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2clbnxilm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uenpplul.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jejealxd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2eaectmbn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsscqqrp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epdfugzg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fsckhmck.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ftisknsm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tluojove.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vtzqxopi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2visbzrqd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rswbxbjy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2oblkvhxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvwmunyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmhhvlkm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhepkek.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yiywzlxl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dhnoatov.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ghnjrmft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2elxhasri.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ogwoujxt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pnmhxfhz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ihyenasq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jboryrct.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qraaomnc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2syncllcr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qaoevicj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qvhtqbkc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kymdtnec.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pronbrqc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ixrozzcg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cvfjubqh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tyedrfzo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nnongqee.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yvvctkee.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lnuxswat.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uxrbdphh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yenddcjz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2toejqmqt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ijixoihs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wfscwgwk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nozxlnbs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2notoetlp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wgrprbag.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2umjwzous.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qcrlblxs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pjabfsdb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pdfvqkdl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wnukpkkq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjngrijo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vtinhvke.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qvusikot.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ieptwafh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qvmklwmy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ocliwrma.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cgqszwyh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vwzcotny.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gkmfbjgt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2inguixvf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qecqipzo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tqbfsvds.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wqrnxrny.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pkevouxf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2klrhnene.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2edzonksw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qrbzlwll.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxhktdc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oausvgbk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2abguprlv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wmegzldk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aggyjrlr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jdzucwgb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptofovvz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2frsovphk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qciitsow.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ynmtgzmr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2oozwswkr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hujspkvu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2umrhbpve.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ypkkqhdq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kpzpceqn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tdecizjm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zcqizwbi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nezjkoeu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2eujaguxt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pskrdmyh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bruztczw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2amdwzyzq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2afqawnlb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ipmwlchn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ehudbiqj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mzzkjlqp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lhapemon.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzrnawn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xeiqjoub.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vxucnnnu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ffpdejki.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2afdkecmh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cdrbqpbx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xchkiovg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tkatcejt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2askeykfz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wirjvabg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vmxjpnwu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2edxstmwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mtoievfs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbokndee.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qqpwfxwx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tatakxuk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mvqtbepw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2laveqjmf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fdmuvqmw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pzjobpug.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2srexltus.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyniwjnz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fhkimlsz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdhssgm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ivwrtzqc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ogjxlgjq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzdleuct.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2crvirpjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gezyzcpj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2garxxzlx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hawodwhl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2twobbczs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fgbforrh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jaallbpt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qtszkrzb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nwfqpujs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mxwahpgr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2heuokebs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hncfwkea.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bkwxrciz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qycztzke.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ihspvebz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pyiethzn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzfltvsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knvomalp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nqxvduxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roshwrlw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jmgyoxwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tkcfidxt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dugegiit.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzsrcmrj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ryaqoqeh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kinvzmtr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2khinyrgz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jyjreimc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jwsktqey.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sawuxdov.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nlakgecq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nglrvqfd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tuqydggf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vbndqhdk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fkbhdtgg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlsrdcu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jcewvqlb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jqnkccpp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hvihyrgn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkjlprg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpzenyyh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qcknayfl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bpgzuucl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxyimjwq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cborjrhj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2veyttlxt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wibhulhr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hewzbdni.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2flwmmsuu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wyrhpbvo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xuecaifr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2drudroes.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnjafrth.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ltvqdzhn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ugdugbdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lxybeuny.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ttpvqtms.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lwvsyhlb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2scijlixb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oyuesqbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fmquanac.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2twcogzem.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2asovbidh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tvegnvgi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzinjyg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zznuhbob.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldibovzi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxsexuec.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vlxydfeh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vxugwhtz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qmzwhxff.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tbaiuxcv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hefcnkov.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pvhtjplm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ulhfzukh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tlwhukuc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xziulnmb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2psylelsd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkkdyqt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfeydzwk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yoxqnrad.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yiqqohlq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpvqbtul.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lxaijybs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jroreuts.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vdpkbgbd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ulehjtqe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bxlodhnr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zsmnpfdl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2igpxswha.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfrlhvco.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vgryeyrm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uawrfwwu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wtkpbimp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzxsdjcq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jkqdpvih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kfigoywm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pqnsrawq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yeeutmth.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gkwhpfxk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2utezjlbr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hrbibudt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2beobogdk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2muxlttzm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jrgmnhid.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrqizwd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fpcxkuov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lmzenycn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2yumcsgav.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eqbnlyoo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2savbrjnl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cydrcrjt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbiwwy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vvnlddhy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ycripksh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twmsiftu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdnnseg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lvfupkvz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zjlofrzx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ypmxbseh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kivgjeds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kytgluud.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovnzgxra.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2prbtshwc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qngprpdw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2spoctjxj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iokwmnim.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gbffdttk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sdagxoby.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yrjcgkes.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2satjtlor.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfaokuua.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzshggfk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jjaqsisj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2aeufzxat.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmteypv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gbolmjto.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rfyftwhu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jslmnnsl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qehjyjrj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oyznzyng.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zszqsykw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tlewihzk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dyvuapms.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ionsnffh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbxrqabp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rzvhodad.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uvbglpkb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkundpdz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ticobkfg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jjgbaorh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ohdnuqzd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wifyjaon.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rgupgsym.html


<!-- 参考信息 -->