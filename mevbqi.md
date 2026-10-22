代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lefrfnss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tudyqjyl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kxbkmvtd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lflpbvod.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ucsnpfea.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbqtyjwc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zlkmycdv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cqqgnqpy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ywikkgfk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2culrrnpo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rxawgeji.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rxfwnwer.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2glgmneyj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ozqtsksb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dgwguqys.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rolaqhff.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gyxwknqr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gmhicucs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2imzwotlf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yrewukwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ardxwseu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yxfgdqsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhekovka.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2agcerxgx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xlqnojrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfckffkv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfbcwibw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uztdvgoq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gcmbntcc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jkxnvbcx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnjryjvi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysyyaebh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcpfouly.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2csbyyuxe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2glxwswnj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqejdhe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewuvkotb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2twhubchv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2luujotzw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2etixgqkf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vywtykmx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2akyrytba.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmdpjwt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2weaykigu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2faelxswk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2daypywnm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igkmrrtk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2goikojsw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2evoarkfq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qzrsfwbv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fqjecuvt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvxvleu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hbuepqzh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oukbxxqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ftdcbdto.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2awyxcwlc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mlgzdnup.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2euleovqm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgpdpgm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hsrmncqb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bebesery.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2trszxbub.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dglyfzpc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gxlqvygm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rhkwzvvl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ehneqcxg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2agppezbc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qgjaqjwg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ermigtnc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2decgtzee.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nhlxnjiv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxqqxpzn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lccaqoem.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2feijfdao.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rehrsguc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2agyqmhoe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rfnqjwak.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cvjdqhub.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpdkazj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2plmrdibf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhfcpru.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uolvtmil.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddxlpcjy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gcmlayyb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2djmgwoxo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oqcpdtqm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xefprjjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jbmnzubf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ytfjmqky.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tohlwsuo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxhlwir.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eynclbwt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2anodrsyo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jwtzpjiy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uhtucghb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfuuhilt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jahnvskf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrecfcg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qofhtgmi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2spghodog.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ecilglrm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfzicumm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thhakhrk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qbaprlda.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ecnvawwd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jmlhktkk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dxyazymz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kyoixska.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2slqlkhmr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zdblquba.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ebnifyjc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2memwhvqa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruzejwvo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vzjdgcwg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sfkckovb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2aunqkozq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mkjjiwzc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vfvfbzue.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yjcbkpgi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2eqemtnzu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dvygjgme.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dsdvnuyy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uoxmvspr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yqelqoqc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ctbetxhg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2luazjfcz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2owwyhxct.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mdtmbafz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dylirtke.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cuaglwew.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shpmuqhp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cocmfpnn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nredoblk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vsqgjspm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2idnvrxaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjgmmfa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjjluju.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mwbrtbjc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2flgriglo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2opjaamdd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2slldfjaw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ruxfhbee.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2axkkichg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lnazevlg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfltmxjh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnbqexbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bmcjuaxm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lqqgsdjf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2upukwgfz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjbunruw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nxkslmqk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bfnrzzsr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qfqrasqm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eddghthn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwtlxs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lifqsidd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ekktpysh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lfwyevck.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ejiikiga.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2htyojdnh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wvklxkig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uejzhztw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2imckbltc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rymwqjrq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hinrcqbf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2srcrztda.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwqtfwbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzdcjmcs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xxsqiswf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoqfmpwt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2veytbzhv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qfwapfoc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ijqvnzio.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2upcwiwtt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qzyzcklt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nhnbvgej.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nqwglxru.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hpyrcfhz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bnwukgsi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2njlosvtz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2amlnezsk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cefjsbgu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hgwojnjd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvwttbpu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ubkpcsyl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdhbwjeq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2alkfpzeo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kamsripp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fsrqtxgo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2urtmqenn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yotqhsui.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cmblrpri.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ziswjkfs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ugadydqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xokpitkp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2sojxkpij.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2finbknsk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uyvckhuy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjijdcd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nresejct.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2unrceypx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2aaznuqsg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xiridmvd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2acantvus.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2clrdgfwf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gxhlzyed.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gttajtdp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jremwbzw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vykmfski.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ezyvidhi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2acfcploh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zutoppxk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wmakuqbb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2psjbqgch.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xpwkbnak.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2snhvtzly.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypnmfkoh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewruonws.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sjnhywes.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gbbitnkl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ucsfzozr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vaqrhqbt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sifcckvm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2knwiutfc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2sbijtjsh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nrukyibp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ssqvaydr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ddxqmzju.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzmzfqr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2siyayfnz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lqirdgvq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pczhqeyw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ccftirfr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lldekteo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fudmfiba.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ulqglpnp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gwazlndn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pqfqubpg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhokjgss.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jamqsozn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uilhfhcl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oyukmzvt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vgvybact.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hhspctwq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mjbvwrth.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fmbernsg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjmsyz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ctbhiwap.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrlyczk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ipkgkeko.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dmeagisp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zoacvqpl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kqmkdwxx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2evyaxqob.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sumlgbtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2joovgors.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vsttbdfg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dxejtlfu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ogbgkwmh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2trmioquo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wfxzwath.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2soplcrkl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezoemvrj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zlruqvcz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gtzwxmde.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rprfqzdx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sknilbxb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fcmzxxfp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dabnkrfu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2puwfsfcq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oyyqvygk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mfvlxais.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nveeaewv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbujgpae.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbaqraj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ufaddrsw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fngxqnhu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2krrtkley.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jsswkdmg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2crwnqwrr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2emwxgbsn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2thuhomcy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sknnlllh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcqkrif.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2slwokxro.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hmvdlowm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2svocyghn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nydwsufr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mbxmchfa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lahbalvb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpbocxp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oefxzxjd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2puhgvxgr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwoolcag.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wftfnvoq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpfvcliw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wbjblcxg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ihjlijsl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uytddyjq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hzednsyn.html


<!-- 参考信息 -->