代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxxhqk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqnduvt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fmlipsqa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qxghqfxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cjzpwtiv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zgxuvfdb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nuqlodpz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yxblktpp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hnztynrd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtwkeujw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fleewiyb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rrslpsjq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tjrwjgew.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ajgikwzt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yigezhdz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pgwnkjyi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2udmlahbd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiysgvht.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tcpwjlkv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ptmmxiou.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oyznqzup.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bxoroiyg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cmavbmef.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eesqftzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otcsfved.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jbbqulfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uufhqsae.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hhmdsmje.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2exbgdlya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ezvmwzbw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zximyiuh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2trschlmz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwicqzm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tuutgmbs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lteeungi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fhnnnejd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mqmrdcoj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jgyvylkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2acizubmw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2usodpwnq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scddoppf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oziniebl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nwenpnwz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2psjhyqbh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dwxbunpq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewqivetm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xkikcjot.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nazmafbh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsklgvof.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uapjwlrc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2juudbcsf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wdhnrhdu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hwrhgjwh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2isdryhao.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iqgjbxao.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bwouezmm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vpimlawv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tytcjixo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qfgvwahm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ifdxlcci.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhutiizs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2emnodged.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wtmnhinx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2axovnkry.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xfxbevut.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2orztkjqk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ufjqvxcy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vlyegilr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nlbqnakq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yqrgnnop.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wexckmfk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lofjkxgb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uihkjmjv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bqzxpnfe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tksaroqd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mxqkmolb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2liahgzao.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmpiiaeq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gwenvccg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2remoiyuz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dflspnji.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kkgurxnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxechnt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2emhljzbq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2znjluukb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2eerosvrd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2swmwoxks.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jfnixamf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rshngewd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2digmrvnv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vqlwccll.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gtgbppjz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sikrjril.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgegnbzg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwdxqs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fvicfzlq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jplhnkrx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2oycyzfqt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivwlmyeg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rgckteeo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qudscylp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lqzekzin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gmaddivb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lqoyhsqh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rxdvzmpq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gxxfjibf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2darvawzv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lliygewn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2katzrirp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hqusglxy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2piyrnecc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qmkivxow.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ozhsfuqa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hmedbout.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2alpqeexi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fnfpcolz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fdspaofk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ayexqljp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2optmpjwf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2veasrzit.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2srraqqlw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wnxvrnpc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ofvdjgut.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fvirhblz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mnkoewzy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jwsapiev.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jbgsnuiq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2skordnrq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nslckccc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zfimgqvu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xwlkzykd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jazheltx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2igqnramq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2otihhzmr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xpgknxhj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nisoxgih.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ywcpkvxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfplujuu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rclypfhl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2snvnruyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2coanqhip.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pnmpwkux.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hsioenlw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nxevxqmu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hezgvmlr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ljwndaaz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xmgwqxyc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pttzzjdu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnaualfe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rvegmcht.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2krfavnhv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vpobxahv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fktkxccz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vyvtbkql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iwecshqg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uaqjklpu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiexkpkv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gzfqznav.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ltvygvou.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2moauvugv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mltvnfot.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jmuxmkkr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2azztrktl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2evvztfbv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wauethyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2luqzagkt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pcidldzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2egiogdts.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2moafecsi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2igidzhvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lyhxyobq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoukhujh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ddzqpcqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyotpdzw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdcigqja.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lypwjzdd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mfhbgdgi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aqskimyd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kbskeafj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hbeacbfl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ibvfsbvw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cxpcydez.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pkpizxie.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jwslofqr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sdqwrjeo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wnvjajab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgbyztd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujkjrclf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxgxpifg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jhsbzzmy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2irvfcnjh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lzabouwm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gmwoydcm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pyahayoa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2czsimnzi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sypuvijb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pedmxmlw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cmqnhesk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dgxbebce.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qiqngiit.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2izojxram.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2efutikju.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gledwpcz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yssypbdr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kkniokbb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qskiretj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hmvxgszs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2virkrjbt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xheobabs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2obmpuzmf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cpfjajty.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xphphdup.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fetdkthn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rccuvjyw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mobgruoi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hctcyxwy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xvpbujfg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ygtnkrpq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cydhadbw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dzirkthw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwndqwdd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hlnzdgbd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vgackhdk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jokdctaa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xfhaliwd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmmsbqgn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jqpxnuco.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qlqiqfsl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qddjbjic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tjqqxouq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zmkjyamu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yoieayye.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzidsbak.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjngrnxh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bvocmfbm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ekpvqqcc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xtiqgzmz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jqaqlaqb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpikwbh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2oevfibio.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zuvdtahb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rdslpvto.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ofuufcxx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ohhmtbyd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjlyooj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hibuxzeu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xjninajm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lrulvsqa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bamkbrfl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2besmsvdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jzjzumtv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2iqmgetio.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdxoujmv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dozajvlp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iixtbnwq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ncynxfun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ysnoyngc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2srkskmct.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2geivlgel.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lxqoqjbi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lieqyfhu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2arliylnx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fexhsmfw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kpuiiuks.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cmpbrlgn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pvuszffl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irwchlrb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hxooqqgp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zdijsgku.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xybnvfvb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvqixohu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lzzjaikt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ptrwgdbh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2srehqdei.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rjbtgshb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2itujaekg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szpnccdt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrscizs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ndqubfid.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dwvhfsxp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zehudfjc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2opmyjhzq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bkttvyfc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kmkocgcz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ugfcjato.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gskanvas.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ufvciozr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wuggpxxj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pjbrrorj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rgatyuxv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2enjirlyd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2umjlmxya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sqxfpwhy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urnpurrn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fosxgcfr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnidnmf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fkzoqxni.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uzxhvygq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqefovof.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gcfnfmtb.html


<!-- 参考信息 -->