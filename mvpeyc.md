代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bibocrxi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2khbdscwb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pcbkcduf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eimpogmk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oclnynfv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uhofkxxs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2crizjxwx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2czbwvxpl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jklvptvn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rowtexfl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dnhkyeeq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cibdghin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lufxbarh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mlpoeyjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nackkudp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gqhbxbqq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yxwyhdwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uqzafnon.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bztnkwdr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2csbiytft.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2feqyxacd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2smhdxwev.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2unxgtxvz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ebojelln.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kqvpnggl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qvnzraqu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2szhhmvcd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnohtpmk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxtjpqde.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tmfsdpez.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjulmgoo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qtcfmtzc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oneidocm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zksxhhia.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rgwxerrv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bvzitnvw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uydqmotf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhgcxgj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsyuwjhb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oehxgdph.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2orhewmjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2tycuzlmn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kuwizxki.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ywngcqjq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffvknmlc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qenzhtnn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qbrobyds.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vrdbcrhm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdozlheq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qugfmttt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vunjebge.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uzajfjkb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yegpjvxk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bmlyjtlt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2byfzpdmy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zcwjvtcn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gygdotnv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2krmcklgg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fiemzkjj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jjecumxa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qyrnynhy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zbhlcdan.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2enqajqme.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2osobwpiv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lqvehiup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ovglmtdo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hmfxmvmd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qrbnrylk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mtrrukdh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lmqwxtyx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2umjgxpvr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jbqfcriz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zejlruga.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mkrzrxio.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dapapfnt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ajlvsemm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2thgbgkjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtpzmz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gokwxuav.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jdeklucz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrroqcdm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fkyuuflq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tckaampp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nzrnjybf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2oggrhylb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wlibnqry.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmhsqoy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2iffksoix.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyipbwoz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhojwyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cnsajogl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jzsxckqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtsdwwbm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2atbvpilz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2poauojni.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jvxswqvq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ukzoujae.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ildgmgpy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tgkgevhe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vtsldeuc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ptwwxdpk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oaplnvjq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bfxeyicl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bftpgqqy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjfimpyv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nbnyoiey.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kyspopzk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wkuwgcak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uxbyazpd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nvenmgbi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uhhyanzz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wiypuoou.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uicaeiag.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rhyyargq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hjbcecsv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2pzzgfjoq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rqyfferd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2osrylnky.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lipxirax.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mhniyjss.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2sbaxflvt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ftwsffne.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xendswaw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ucwqtrec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lyvpztja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoaixrpw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fdetqtrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ugwazqfp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mxzbwpxy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ufddprdm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2teoewrky.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ladjgobx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xowhdbvx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wsniyqqu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2twxnievd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kakbphxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2isftflwi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2arqpysoz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bmocavof.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zzpxyjks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cxzuuxbm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wcfgxyys.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kvuudzwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fxwldgbt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wryrknut.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2oaelughh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bceoiyst.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gptkahwf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2icoszcmv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hpevgduf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cisnilcq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ltzkgeqg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hrpjdojc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fpmkusjq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2iqjvqrwc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bqpevwbx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ajnqsosq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tvoqmsds.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgkuuhyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwugfjuy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vnlfzjzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvsdsswy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rvmhlqlp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yphpqemb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iwrgeela.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zqaooeiy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2omagzacl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2klxpkdvp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jiqorrrr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rjwplwcs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pwpzzaiv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nnbjamrp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kkwheshj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2iudyncvq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2afbjedcp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqxqeuwj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lsdjlblw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hlnjmkop.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nhukheqn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwykbtf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2djdbmkrm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upqrieby.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxkxwmxs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kzrqnrtg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2shknhvjw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xmslllcj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jmkksdbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2verrhhwv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2demgxgai.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nilwxhlk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dlvmznuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tpklfhib.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qryeyiht.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fkmbekpm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xbnqcvye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dwafwzho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yfvjhfew.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bymkwexc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wbkghuut.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zqrcpviy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vaeypmqk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2agymddrx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wgebreos.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ruolgzpi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hhcrmjef.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qxupxvtp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yeudazor.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eeoafows.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmrtljxr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkcxzrao.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eqctshky.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgpxpo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dllbtvyv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2paclodqf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nggcgljz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hsyhqcjt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvedlxby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dtmasprh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iiyeyivn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sbrazbgg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qtkdsmio.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fuxywnbv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wuegamty.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wviskyum.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fvhyusma.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vlrckups.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2soxqpthl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ojadvhri.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vphrocrk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dxtrosvt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mzohunkb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tqlsekov.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mutinbwo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqcsif.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dvbplvdl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2osauwqxs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqyalgzz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pojspcrz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bopaqccm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xqzcgwlr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uiltutdd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fbkbwdou.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vcnciswk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2calggzws.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gztssnpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mjkerecb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bhcyqwbz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uwebszlq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gjfzjrwc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2skmblslg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xgijsxmw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2akdavneh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2odskfftg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zhbihngu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2sukzyqqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nitthcdt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jzodufnq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2llteqtet.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fztayxcx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zfgrnssr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wxgvuwmi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qrlqyiwd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zqjefnzl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nqgdwflq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtneadrz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gfnxgsiz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mnxixyay.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aokhsnhr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rvrbhdcq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qmeblrfd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qrfuubab.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2irjfcgfx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmteiz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhruvlps.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2izbialts.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xledizde.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2izevkrzr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftyoqyid.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2izffjixz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nrnxanxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lindxvmr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sbzhgqio.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdakmitm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2frhdntnm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qrxuovyg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zilabktl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymduwfym.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdcsznfa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dahlfmtw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zimqigvu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhtvwfra.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mfmhwcno.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nhpvszoq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2debrwdgk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tvkzrzii.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hckudkps.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gvktafmg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ntsjkzng.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xbicuajq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2holedszh.html


<!-- 参考信息 -->