代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ljzgtqop.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mhbfiwfo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uhthoqdt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rbodzwaa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hladdxtk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ouqlbucu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qtedzyls.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cbrolgth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opwpticu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vbaxtxlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfitkiqy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3prduuzrj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cmxmohkg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juwtlsns.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxtqzrmi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcdolrkl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wlpaqlje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iaywemdj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yyvdmdsk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3goybgsti.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fniacptk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vuoidees.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gxuzqrtt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dslckezd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wybkbqkk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pmcfexoi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ieeelbzy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3uumxroam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pwxotttx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sqdkvetq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ebpxjufa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bkwvduxj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnabikp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlprkjvo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3voratdxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zzdvwmxd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3khkwpwmk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vqnbkseb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qjxvusdb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zmkzkntg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xkwbmkkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3txafmzhh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3erckmvdg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tweylvsm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3biniziks.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qlkmxibx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvbquhc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sqqdlebr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gjwwwqiv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jsrrkzdm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wapgftrq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uctymoql.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zsmeslor.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jvlpadgv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qeuknlge.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3chjqfcta.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3akrwisii.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uydfgvhq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pfhnwkqd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ofghknfp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kmtnvllr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ilcubsry.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ygrwzmyi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dzzulytu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jbeirzcd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vcijmczr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuayaoq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zyqyxvyi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3mabsyuyk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xgkjfhji.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgneyovh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kzjujxis.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zutthsqg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gjxfifcx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vlnnvayr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hbhulpsw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnehmlvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3btvgzntg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wjmcgpji.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qsrztrbz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gorngcym.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3opnffrjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iajhdgcx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3sedplmbd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bcwfjecs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gryhpyrw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ehnopiho.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gplgwmep.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3epthcsuf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3oxhtlojt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgrsbbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3onjcoahq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lmkoikqx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kfbhages.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3uutfxxxd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3edlytlba.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sqfkyxsk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sjmnfccq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qzyijqub.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zddakkky.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qpymuiqx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3djwbprdr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ijvdbhhk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qjchmjxl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3chwzvoas.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3frphgxut.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rdlkuojw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3akovazfx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3csckwajn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wpduiijo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3layewiie.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kpdplbfs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kkrhzarb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wmwvghcb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xygahsaz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aywawewc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yjaxqtfk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qisnmeja.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qyomgglz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3finqvbwx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ropyraco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfroyieb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qlzeuvsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xrbxngff.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnrlbclz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lnfkuojo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wxocjwtq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kmwgovir.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3igvpktub.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zkbldpak.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ptellgjl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uelivoim.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwifihin.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkwduqh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gzcugxfo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3epuzcnpu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rwejbuld.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mjsombhw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fukjbfck.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rkyklatp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xggaciij.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgobelnk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tlpijcqe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qukqofly.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cevoaidh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bwkzzjsn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hdwrfiye.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kvowsgxb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3shgikfgk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3srxamrcq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bkgvnhql.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adveyzgm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3eqdthibl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fozffhos.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qfuhvnjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tntziimg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zfokkiwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngmmfgye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zcnevztj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qzcvnfla.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3luocvnqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gyxwpgpg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gqprqtii.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ukxosqrg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uhxmiwka.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylrfcqoe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nitalnrr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3snvyezpn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bmpycxsj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qzaofchk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gefgsksb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jpxsnwof.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwxfhajn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3byivpigw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lpksfzqe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3glmdsavc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hkokcgby.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkgobww.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sbeaitpo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jckxyhvi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tptfdpkm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urchuhqw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wmssgwmt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hrnrobwp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nvjcrtvp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vbaxbdnq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgolguwy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yemiisld.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ewfftayu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ogpizzbc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkynuvzd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sjxntxvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eehqmssc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukzyuozz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vizyshog.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jpaybhgm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hrqphbsr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3woslysfh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3efzoawtp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3loqnzoty.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ljbfqwft.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ijdlptvq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gopmyquy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dlksaskk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcdpfigy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puaufzki.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xjfwpxii.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3idmdpgbn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jyzmgzfk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqriamls.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xeuwtufr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3aulyzzym.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lepatfdx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qxqqzcgs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yppzbmky.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3adwfrjlv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3isgrifez.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpryeibi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jcompbew.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ugmfhrqt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3clyozfqy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgbmkx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nikpjtnv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fplzqtww.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vmfrzpll.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vxobfieq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lsyumpam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ncmvgqbp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3olvffiow.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ufdmzwrf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gosrgnlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mjoaarvn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlsnqp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bbopqzgv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ldbdkdso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tverbfst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esfgmmxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gxjcggfy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3unhlqcnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jtirfxri.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cyibpgcf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttqrwpbg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kvqwxxdb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hmfbjxyr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hlocbyhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rdalqiia.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hnncgire.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gfkgfxzi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qrqzhiii.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fojytkju.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zlvbkwyv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fxdxlxnn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3brabfpfm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ltconfnr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mplstorz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zxkobrjv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cftsetqo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bjqvrckq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zpgdnviy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbxilquk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pmxbzkty.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3roxrrobh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xyoqjyva.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zktwnlci.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ncplhcww.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fdkuwvnv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ifmlawpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tkkewimi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3thldpiuw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3joocgsfb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3smhgrhij.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fktcysgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3aybbrnhm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bxjuiogx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eonffdpf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kvwpfhkg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qulbxsqo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mygynhgs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqakgota.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bvlhviti.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecnlacrv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3obeydebh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcmbfghn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sfbpkybw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oevwbram.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sdcqzkma.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oliujfpl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqakvh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mwrhhpnb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ydybtxvk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3prmrpplp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cwfetnum.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ikvaxzin.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qkgivthj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqwdthkq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3klzfbebg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fttlczmr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ruofnvvb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bhgoqtlj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nwnaiyul.html


<!-- 参考信息 -->