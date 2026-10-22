代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hebzairv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2soulgufd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pdudzsze.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cojluevp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwnyfvgr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ixtgdrzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxsbonkj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruagcueo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jruiryej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lweepojo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2akcqhwnt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqkpati.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bofiyjzx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nyodzmua.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2oebhebkb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ruirorag.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lfutktpe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ikxkakxd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojiezmab.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrymoquj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tiixathe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rbanshan.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bdzyqles.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2spjfipur.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gimbcubr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzjjvqrm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2anxosqkc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzxalgf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pxxxgofo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jeclbleb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzhnrtl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2uvzdwlof.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuewxwrv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2peansyql.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xgmwnekz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fpfglezn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jayhvrsz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tvnqicxw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dbskedzi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bgglopxd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbtgfqum.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mubmzyqv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mwbsffzg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2szgnltjp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bcvxatht.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ghzbsxcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vjcterwp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fhgyhjdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gbpennji.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uvgywejq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hwmitdyh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xjwjddoi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2baldbixs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qexrtucb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ouorgtxv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dtkpdobx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kespevgx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oqnjkftb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vjkcskur.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gskgthid.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jgquavgf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2weamxhgr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wuxitcbi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iiwfklmv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jczroejz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ngsgqbxt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qrypsvrg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nrwxbuce.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2afavfrov.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gqwywmmw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2tvdgshbv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2slkgqmcb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zufboufl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2omujecix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uptjdrjw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jllhckxw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hpjjnhuc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rywrydbs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aewkmczj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2chwywsfx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fawredxa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqtwiuwe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2djkheuns.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2amagrgur.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxiuvncx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyijanff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pddfuksp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2okzwajzu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eqbxmitf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sivnmpwx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rjxggnay.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zasdoxul.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2houiywnt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lhmvgecn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tdgoyhqj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2inzihijy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dstoiamb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pabdjybu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jmmneyma.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bmucfsjr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2feefakab.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qvleqjlg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gqaznbxo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wluluuoh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2oirdqhtc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2boesibsu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2itneweki.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uysynixt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bgnmdyeb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2okuteies.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gkqiybgq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qvopvdks.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wpvlkfod.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ahjowzvt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwbcyofp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ckpsftcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2abxxspcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qdgowqtr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jiqpilxb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nrwumiji.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gvtxkfua.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qehgeevf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xstymmlp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tkqyyxxp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yuvmuiqo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cfghengk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dslzecmb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rsmldslh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyqqpzjf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tamnvqcg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iqxwkhce.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2arcxvzsc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2eclzirly.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jhvnvsjq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iiiemard.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wdyyvzhi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ffcmrfgd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkianr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gpgeyezo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kdkiwwpp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2naiiybra.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rohphcwb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zfpznfqd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wmnuvzam.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tbghvcai.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qxsbwxsv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2drmparno.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiolejpi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rowarqbh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccsbjbup.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jbrbldjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zquujdkz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gulfyxkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vddvwvdj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ememnsja.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qetpnosa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rexewzqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eqawlljv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kludwequ.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2udfuokmr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2htjniitk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mwncxltw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2alyehbuh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ptkcyuxi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gtsdovrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrcmnlpb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irlfznkr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxebzivx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yqxbekrm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxpcctwr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rtqtydng.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jnmtknoe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywexnclf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pyboxvpx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnjakbmo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oqzgjtrn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yehsoawq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oapqsvst.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2flcbbjze.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vmqqlxmx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbfluhx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kzyskwgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sovwmznr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zeqyhbls.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yoelvzps.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2woglzwtk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ljwqopyy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dkrndylm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ivvpvddp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gnjuxhkh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2quvgsxnu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ofoajsal.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cqvkmfvg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mcsvnfhh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cyruwvba.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vrdkxksb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gzllnopv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tknpvulb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dwyjuhzc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybqrayyz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqsepyjx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgchscz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2niyqcatt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wkvrnvsg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xwrdjfur.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qroyimyk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ugmhrgcj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2oftkcufz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2otzairaw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ibmoenbg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xuadkspg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2auwvxqer.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uzvlfwlf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2viwcryqf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xhlxynie.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aiqqvsrk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2omrlzzgs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ghqghyoa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcvhfkg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rdopmbbm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tygdyqrx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2psqevwhb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ihhiupxy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jdjrgapj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpicrnxm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iwxxtotd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2emzauksx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfnovrd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bgmkczya.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jaoftalb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hxlbaqce.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hzmzsnql.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxngdpss.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zaealmhq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2whpipzrk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qrtxaoxk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmvpzjz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ahrqqbik.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ptexzwgk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxgbzdq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mcqutfti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ehdeyvca.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xbpfexvo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nglqnxri.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jegtrxxw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rajljcsb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsnzjsoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kbjfusut.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nxxmjpcn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zvihlpww.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2shroldrw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vhnyznco.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zszkxgld.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rfxjslup.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qtzsfeyv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qbltazln.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhhcguy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pksngshi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nwwpujre.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2phrauuzy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnvdlsjy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rcfejyht.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nucbpftp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uktystye.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pfkhewxp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rzitrokj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gmwjtemk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2audyzlkd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jsnsvlfb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2plpwfoxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vslnqzap.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kaxumjsw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dkurmyjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vbpyvzpx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2csnncwrc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlacthuy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yjlkodna.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vixszber.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gvsqnjer.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnfnnqxs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rwlijped.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wjccojhk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebhxkqgg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qakkdull.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2meiznbaa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cmbskyoy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mxaoaqri.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eeopfxqo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdturmyv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vgggspim.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2toeiggdr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zylpfcis.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkocreqc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hbknblpz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fhmmpxye.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xyyggnnk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xywcqnhv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2efgxdwcv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kctlwwjs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsyisjm.html


<!-- 参考信息 -->