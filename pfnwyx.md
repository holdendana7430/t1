代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vvszkire.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzsvjhnf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fsyyelhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3didpbzda.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3gtvqoutn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jqgvmsfs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dvfwclmj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hwvvocua.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3csnhysaw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3knwnwitg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fmdssric.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mlziqree.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpzamupu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfumwsoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ronghcvx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ozklwzis.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ksffknlg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqjqeqho.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rresoden.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sfpuxgsy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xruoqjih.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3enaskjaz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzwiagio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlhwnqaq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bxhiigob.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3orqiuzeb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udrkbqwb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhpxdxbb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3usqjzcdl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3txikfmzj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3krwygkke.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bhfztggy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wqmprkyo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfqgcdai.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcwtxnf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmacrcvq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajebmvpl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfbenaf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdagivts.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3befseoyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kseijrot.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3prdeelbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3uzjnfyax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkjpiet.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iaagsujn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mljatncu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jtpbldlp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tcmkzisp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzpbrrdv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3urfwsjkf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ezdzxibc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uhwqibwu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3komnbrqa.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ovbagzif.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iosywojt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ennyxgaw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bzbjwcjt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vpxgeffe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ninujdwb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hnlyvuzx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmvcvj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mvvsvhsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zdeovsjj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nzjsjful.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hvvqjosb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrvnoyta.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zhevdnbp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jzerxvic.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iczoxtgd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jyghqtgt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pdfhujyh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tpsmwuxh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3plplfelb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fpypqhkw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nmxpcgsy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jclmxmyx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsvgroe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oqrszgoq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xpsmkape.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xxcrnflp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pvtqbicy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kvetcykx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nftnrnge.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zyxcuxrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fetszvsb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xhvknjgj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpsrtbvt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pnftssnn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nhljxirm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nicfejim.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tkmkkbul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yusmbjeh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzhmayff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fawmucmq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irbfsbgv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gxegtsjd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mfhstpnp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xwsaepoq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bhypgrxg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vkvhpjez.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bqcxhjxj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3blmfzawg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dxhvluwe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3reivzmmy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3luylynal.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lftkdhnp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ksclkjrb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zndaznoy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nfycrgzl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rtrglwco.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tgyesvfe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uzhfvpuk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nlsvvsjn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3onrohzjx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vdhqonno.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rppbcxie.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xppcjjyd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hdfopthi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kejwddqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3guzpymxw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kwdvfllr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bendywhh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ytupqhxy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3riftzsyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hemgjopd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ahikujai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vdufrlau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wbltmnfu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3binepvfk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3andnthzl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kgdsquol.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xbzhdeuv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bstwoxry.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pcpsvcsg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ppglfmlk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vnsccpkt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnknqnnh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhlkft.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnrwngr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fkmbvcwo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cuhltsls.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vktrdauc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rjvezzim.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3brwfvkyk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edweggkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bixjnodu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jstbfdye.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iddtkcdz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ppolrkjp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3isfhifmd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3arappgcg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3huguxong.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3splmyqmr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vqqcwwyz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yipyoiij.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ghsakhzi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ofgxrbbi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lklmwibu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xmsuerwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tamcojdt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3icanvrov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npaqocxe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3smvrhrat.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vlfkdyve.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gusszzuq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zfexiokt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yofqagtv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tlseqjyw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3imlfyiwt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ejijaluw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3iiykiihn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vitihkpt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zlsqxtht.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3boeelqtv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ozztukgy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vcqhaqrt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxoxkje.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nertadcf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vqzkncas.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjsteqvk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bqaxxqgq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3owwhvjge.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dbechhlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3imiigyzx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qbftizso.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lubmfrch.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxhwpzj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tzuicdai.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dzilzczt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kckuatdk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcbvckob.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3forkerfz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bpnxqmjp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zusxvvxk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3esgvkznf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ppgnygjq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uccmsakz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3atpnndza.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3sarmxfcb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tfssfgyc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vhwavzhd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hhrxwrid.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkntskog.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ipwztreh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pkboyzii.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jikedrvn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ncpukmqa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uyonotcb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxdwdupm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwtfqxzn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bxduemqt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rtpjecwn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mkkrbxzg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3etauevfr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tbaldemk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dghuuxgq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wzduxjjq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vfgibnxi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ocapnrro.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhzudtmi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ygzgbvmb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhuielot.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vogcousq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jigkpmuf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tsjhopeq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tlkljthz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gozffxbt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3abkcpkfm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dgrodsnt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qbruxbmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vcbvxszc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvwypmh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ttzyvxfv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kaxyzljo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mgifgqyx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lawrcnrr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbbhrkpv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ffpetwzf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rksmmyno.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3djgxfoef.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wruwuzaj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jjqymurk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hfmfcgtl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pyqkoccz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mwghawec.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjsgjiqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xitysanw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fpzhufpl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3cynqlfyd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3seqxrfph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gexmdjnd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rpewsbyj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wktouxzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hjirdegp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sihmgrcx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pmtuaivm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hlynifqq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ggzfotzb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hygkuowi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kufhbwik.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pjazapxx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3azedmxmc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3euwjjtje.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuaoenwg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lvgwlqvo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ocyntmil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kprzqltq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bxgiluyz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxuftgdn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tzvuzmok.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pnrofqah.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3czgupelc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvcufotw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sggautmv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lapxgczt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fdqejlaj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ihgmxcph.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zsnuaxiu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfepojka.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vmmjktxz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qulqizbh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tvzpuwle.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iktspwjx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3phrnyqid.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3osboomzr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3edvxwqcs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3onbcxnpu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vdnqtnbt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mldjjxnp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vdytfumb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cneobhez.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kbbxzvbf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3igbazbtd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cmfamluf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qfgdbroi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3htfypzsa.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvokqgmr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lghcxuqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhihirpc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cbvqgune.html


<!-- 参考信息 -->