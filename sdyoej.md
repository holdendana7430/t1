代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uootmnjn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwtddpz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2elweqqae.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjzadpn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jabydnzf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgxtlzbv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqzzpn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2anaslyof.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lmnftabz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dizjvrxj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzrmfirr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tfssklot.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dzexcbho.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aninwzag.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eyvuibhr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wpoxeqyq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gdwvnooa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvzjjbkx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tferwxfj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lekbpkjk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bmhzlhew.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hbtqqmwq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2foovrxjy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lhnadsso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twerouna.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vesnpzmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmmbohar.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mufwxiec.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rxeybqfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfappeqe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bffyadcb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hkcfrcmz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auadpmvc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2azqkzope.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmbhgjeb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncprhahb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdccvxnt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2oleqwbpv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wckudtaa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eucjpeuh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ozmhjcmm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ajendnwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zyxchvte.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2daylrfkw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2urkpduvx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jjwflhih.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nzklvljc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tggtpibv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mokigkkj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fbzeqnvk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bcznqlhe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cyleqbzl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aumuqvme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mrxedahe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yovvvtbt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fopuotsb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2okvnmgcz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dtttmsit.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwtnky.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kfciofag.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvvgniie.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iflmsuhk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ghfepray.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bjwaytpu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lzeojgub.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ixtysbrj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2svijeqnj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dtwuuhxk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2edknhhln.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2llgiocfc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xmlekhci.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rzawvwjk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kaoqiqcn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qlaayjso.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mjsiufgk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dbqrtfne.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iideppbv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2srcuqapm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wejgzkkh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cvkmqbzi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jcakbcyk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yigfnyld.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bnwtaohc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxespfql.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gocxmzyh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ueymtsrh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2avxgtudx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gxkxmivx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lmlpnpys.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2edouehqp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hjexdakm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jizxilhu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cfapkncp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnsuwsfu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wuotvqnr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gugknoso.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dhfdpqjt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dxivjunw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cogidaza.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2foihqfqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2plmzyhcv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2brabjijv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cuqedwig.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2badsbugi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ypvqepae.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdntxjt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ctfwbztj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ukyctfha.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xwntukjp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vwgukvxb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ihipzfof.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zkaifmaw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2irwvbtsc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lqrnxpka.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2masofqmt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uzwpyvxv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fkcpygef.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2flfsztbc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tvoboxzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hiklljcz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wsimpgpt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vhunnryy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uywrwoyp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ysenplgf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bkqrybbc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nhiavdvg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zrddygxz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2teubkfpz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wmaazcad.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2twiogzyn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xjxiwdei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rqttphxp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mkufdqil.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kitvznra.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbrufh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jshnwwvq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2brrdpjen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sbhidgms.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2elawzhnt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucgmvffo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkfxibqc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vdamesan.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mclivnmy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xhhckgab.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uyrtbnue.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2svfxkypp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xdwfxriu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cndopaer.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxkjwinv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vokkzikr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2avacluqc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bwxuadit.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ukhibuye.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnjduibp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lnspyjya.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rdvkohnq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nhiogjwt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbjhbggs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2welhsyxh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iegscmqm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kotdzlix.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gtrhxcgp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hyywmjjy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ncmjlpbu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lmyunjpm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dzciekfk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2crakohck.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bwyhadzq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pknfizpk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jcaqweud.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orpfxwmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omlagxwd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2msqczpvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffrakbmi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bdiexnnk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pehjnddr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2adoanrdn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2odkgytvr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fdvctwje.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2odlnkaiv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rjlrcvuf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xwyrjntw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jbcjnmsh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tmituqmi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rkuidsya.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xcazariq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qhcvouhv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xteccyly.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2leuyshkz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sjnfsagq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qqmvfngl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbzclvpl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kyelxghb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uukurffa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkobbdpu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ejbfmnow.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vruhrvph.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ewjtwwpl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2klkvqjwx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qottxloz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2odkjepiq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bmuoytum.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mnmwjgiy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzafajkk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kkeooayo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2omxjmkoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2moandgah.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtcminf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2baecndwh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rryiylut.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdsbtzvm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wddpfkon.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gchlflps.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gtycgulv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2muvnbybb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hnolznmx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ccfitreh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zzcvstmb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xtattvlw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dqnztjjn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpubimzn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtwvsmlx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvrxseva.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ylhsxmfq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lbngzgtu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hoixfgfi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lbjreopp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wntvvrky.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tkqcanwg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tudarwsj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewcplhde.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hrlvfllz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fvksqdfz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cgmojrzh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2atojyvgi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2irnctpcd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sorgpumy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pnpawgtw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fjgsguis.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rdrwbyjk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2csjjbdiw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ftahxzqp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qchgutyw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqrgqjb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qkqfkjzt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfahdjdx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kymuvkjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tbdrfzvm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsxeazfe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aftefazb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zhtrvsay.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdgqckr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yimljgvp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2whfzzudm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2flgtorrx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tlvgxjzs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qeebdqxg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvvaegpt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2azsfivhx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hmtqnwap.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bkmpzbzu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2flgkdepm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mzlfwpaj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mubtbfzk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xjiywkvb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pyfvyxhr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2agzxrjeo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ruztkmju.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xdrldaeu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cvicxjoz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijtbxrcs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kjxryhfe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2oumtqmkf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oioefgwz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nphkdrri.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dfhouqlm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2engmzasi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2krpeysfz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gfhlmmut.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdiavuml.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jaakabgo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pewaiitl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wigyaupf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lyygtzbp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dmhlzdhe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sozyagxw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmltfi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ktrqwamp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vzyyxrrz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2luskizpn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtajqajm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qxwfvmow.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2agmzwtkl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itlmhzwb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyedpagf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qmvuortf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tejdcitp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2txezkdct.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ycmqzygh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rfdjauyp.html


<!-- 参考信息 -->