代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zjjilvjv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gbswdbdz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zanqgvvt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fpeubnrv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bdxpmlqk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qgmpbyay.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rzdepnrn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wingctue.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rqbznakx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lsiunotr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jmjqtgtl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fnlgpxpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whfyzwmi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bvasyxst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dklveegp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqqkluyq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gcmhmftb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3khyhkuit.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3piwictrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wsyhubus.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvipxpmw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kebtofpi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3emqlusxm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rhledktc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kjhbiymb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3obpivrye.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hqrbbqar.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpqnmbrl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncnizzvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3isxsznba.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3acucpkzx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xhewqffh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ymmdjlbs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3flakyxbf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpmbfcq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dsvtndpr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3abclpjen.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdduxbip.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3iiiuuzzi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kymxwnpx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgbbiejj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sdsgqxpb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ghrvvutp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3eacjemxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3beyizpdi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eeduvfwy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mbymcwrj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3paymmdjp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3llxrkypp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mlurmnkq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3amsfgzpr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3abuldjea.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bdsinhvx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lemfomyu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mmqjrdjl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mnxjhran.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dgmboheb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pddbdsbf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pzajrypd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3balkrhoq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mjsafqob.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pzuowpjy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3biqflovf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ufvcqahj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kwkkbjfc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3trqvwayr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ohohgnhg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3krnpfdnb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqfppibm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lpgchreq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fufjwjox.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oujjpxsc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzjgtmt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3adyetkfl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3znmdigxk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yplprxue.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtmrmfn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ntltfaut.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dppytxca.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3duzcieuf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3danwchwn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3diwpocjh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gpakkzxb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3eemfyxzp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cplmsdlm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfgklucz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pkhvethx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ipwjzhwf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tncyvwbi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3frdqeqyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mrjsexsp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rexbpfez.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmdeosq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pdbertpz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3panibzrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ashknbmz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3obxedsqu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wonabofy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ejdhcsdd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwjgxwnf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rqjyjrjc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lmuchwml.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrbqarov.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3apjdkywg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hboendre.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3prcjikmd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3sntxnxde.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3erobsnta.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yrkaqsvr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ycuqcwzq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3iswkmuxr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3inzpdqrd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qcvdjeqi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fqpfflea.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3aoqpiqaj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3crqenubd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3erzoobuu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jvjetpka.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3msqtshxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cquvwrso.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iddhexna.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ozuccypj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3fnihbudj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ytyvdikz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zoicavyc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xrizmvzv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xcwypoei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jskilvee.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yeesxdzv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gydkebsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yildfhoo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3quhhimwr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xyvclofp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cyctxrwr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fybypbsj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wefkyhuw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3elmdjrhf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bitrqdxl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zujzrwbv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sgdsofdo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3palbfdjt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gojrjaye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xluildgx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mmqynhrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jhwuznzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utsdruzl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cqairnrd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dbrwvdqp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cppfjnzg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zihxvsnc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3irkmgauh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gyeybvha.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gubwhhyl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fuexksrd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dipqdqxo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ghqvkjlg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dwesuntv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sqtittnv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrkrqlhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vswmgeqi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kneexcys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjrplypf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iryipajp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nzqlpmwz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvoqof.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iokvlthp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tqxfeyvt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ardlcrkx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fdtpodqx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aijvjvks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3alsnphsf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jcozszrj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hkvpjeak.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3exwetczd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cgufcnuo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zvoknvjn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3gkchepxb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3evmayczm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3titlglcg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xaksfgjv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3eyrlixyr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3elcrnnic.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eieivthk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wkikaist.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3moqiylsf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rhwtavvb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wodcxcuu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zvjmcavo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ubsyjqxl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hclwosey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fdymfzsr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfxhmiwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3icqizftr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3epnatvkb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3megivyhy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3libgpqso.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3favtavjy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnbupqy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3juoyuwus.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3twasfuvk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xktuccjw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3abrlbdsb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hmyhjxtt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3makbtqqz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rwqbpuma.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fthbdozd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pdjaksyz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3waylhash.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqhhoeol.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ondrjeqe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3txrhbmzu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jupdnpkf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3teshpjpq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjvwxwob.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gjnepmoa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cfkuzktx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3blkaoxvi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3koeemqyq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3suzqsflc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lbzkngnn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qhmjzjzc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kjwddlqz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yzovhhbv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ggnbhheo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fsvzwqee.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zcnnhcop.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3brweytzb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmzxahk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jlsqdsak.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tjrmkokw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkwtauap.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vfdqazmj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3afmxitrj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xaihcxaz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tpqvjolc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fnncqjxs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnhwpkfq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ezmhxqln.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3peyxywxx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yxzhepqx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqimihzp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wdwgupqg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ahulsbjy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vzrfpvrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fennkbbw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dznmwfly.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dnyjjezs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ipsfgvmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3osagiydk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ptllduqs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qmiwcckr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wjsmzdoo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nbbpheht.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vcqlawbi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3aqohywoh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lokvojcu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xjqkdzbf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ohfgovch.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ansmwzwv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mgfjbbwk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kasfrvdw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vpldgcyc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tbndvxli.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uqvpiabv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sawrbwqm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dtorttrl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lisjmcri.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhffdeyg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fjgapqlz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uuonavst.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aizfelkw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3flzhboij.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3coftpoqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vavkifxq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zalcpsud.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hatdnbyk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zkbiwqxt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkislqpi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvhwlasz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pxmfqggb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ucochkvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hupyhknc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ademzdtl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbjyole.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhxetiyc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3whjqxdbj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vdjfzhhc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rucuebsf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kfpchsso.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qcocfigo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bclgekve.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zqjhgpnc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eksivbde.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3oarzzvdj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pdleseig.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3chctrvot.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckqcvynn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3foavmyal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tggougoo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azlhpkoq.html


<!-- 参考信息 -->