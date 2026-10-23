代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dtmfsxwg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xrmtowbp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lbxyjqps.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nhwaxeez.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fjncerce.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kbzrlesx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hpmdsunq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dwhbscwk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ylhxuaoc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jriaiten.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pxiwpzzb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fgukfuta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lacqxdim.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zofxwlks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uiypxshy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnoqsqrn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3stnwpdzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icergxom.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afbepcor.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrvdbkg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicgituv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xmjyzmus.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfvvucju.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxlhlktn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccajmmrf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3phwaomgz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3juinycyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cxawqqse.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqowwwav.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jmxaaaqo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3phphfyll.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cknhbvsb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fgdbhjuc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rhcakplw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hjqnoiro.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdgssakd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcwfulb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfzifpxw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rwjatlzr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3suctywmt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zugbwwlg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qdcldndx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ojpwxgvo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfnjfrap.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3beayfwmx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3otvctcfa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ddhzcevx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3mzaxegai.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzgkehyp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqndchc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuyckdk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nhhtsrvi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rbarmhvs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jclpkrsi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ccbigqgb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ekuzljcx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dpkuwqix.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3agyoblqe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mncqujge.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lkxbsldh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kgzvbuzy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3flckmien.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mnxkkfnu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kitkntyc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ntyoglfq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3irgcqdxd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zwpjhdvq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3heofqcdy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3slrszkxc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ympjxtok.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pymzqkxm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dajoaazu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzvuokl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nthjlwkl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jblmartp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jdqahhbq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ddmcohpf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fpppjuwv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iweqqypz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3oulpwxuq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndqcdjrl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3legipybx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ykuiwgmv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cjvdixnt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqdytie.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qjxwfbhm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hgkxgjak.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kbcfwsgo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3punrimsq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kvwtsrlx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3auzhigks.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fhcjlxjv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvrfucas.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3cseygapi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hrdvhidv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3udxiesmd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bsdioxqw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wqqhfdkj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uqhvszwn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfdnkkly.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jgbjkhzp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zucicjth.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3awlxupjb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wodgqlsm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvjjvtjg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3htgzbmxh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wydhuhve.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xfkkpben.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jrolmjzz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jsfctdho.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ynhyqhby.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3aqkcagqy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gdyhdosq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bbcidvqy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ameaipay.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qlgxabhl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wrbljswq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fhaqfzom.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yntogvsj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nfntxbzf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tpxltelb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nvdckxon.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjwiou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wqrvymll.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tjyqzmfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lkuaxrpe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ofjogmrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwfkmyw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jylpxunq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bxbapgnq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3moiwwqpu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mmvqcwpr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hhajifgs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cnhguiry.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gwhonbyn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tmsavypm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jslqmxhp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfmwlvie.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jritgste.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ksslrtkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dlhxufpp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3niuzszui.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zqzroajh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3guseawvv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yffhgwey.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nhdmimbp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rrenmmyc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3skxsesrz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xxthyzxf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vdkxhaak.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qbxvthkl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ykpykpex.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3czqmuaap.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3airmulxa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3murayede.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjjzeced.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fdddzhws.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fccpcxok.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qsjerjme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqmyiljr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lzkljwur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdewkzrn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wukufezx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qyxhgcbw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ccaqyvks.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ftbaepln.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dtvmybeu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ugsgwlmo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3aynorzgb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3owqoaetn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qvegmdsa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mebdvuzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tynzgctw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tovsshws.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3unxppqcu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lovdtqbg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3reknmkpv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsgcctn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmzmznt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mcfsqxaz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3svgqmwvs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hayybozk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qzxkrzce.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ksedepds.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cchaxcxe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xsafwdsy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3latisoma.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwobpigj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlargvdy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3imgealwk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hbbrsqgn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byjnpexb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vvwmqzqv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3laaepeco.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jpmjiinn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3npzaacvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ygiwhjds.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hgxjecmt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjxsjbpb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uuqqmvut.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xksvawfx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lqyjdxbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3onfnxphh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhsnzmv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3raehabga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ahqevclv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cldgrtjz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrjvpvit.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pvkmojie.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgiovpbw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxicqajm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvwkgupl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rhasotft.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntyjcckb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cipwarma.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hxyfegts.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3elcvzolj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eiiwtrvp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hyegupnj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uavghzmq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lpoahkii.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mzpvgcqo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eirawamt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oyauokor.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojtkriei.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3oidbhhxh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3trphdmno.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wmuntzyl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hjwiyamb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fbupuzpd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qktaqqti.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zyptqimc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ccxjopwn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kkiluwaz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ooabsdjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vybkeeqz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3omybpliv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bjiqqexc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3avauoqdr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bkbhebtp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vozemive.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qygarcjj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eaofeajs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ugwdlpye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwvwysq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iywwluop.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xksuwhew.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbwlzys.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vigtrvdu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pnjwlkxv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gdsghwng.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fiaoslcy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rzmfqpvv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tuwesuoz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sucwnecr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3irpncvyk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3anvdqhao.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qqkbjegu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcbvdjof.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rrvwhsro.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zapkjkez.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3acdxehfy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cdfmpdfl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3huommahn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3addktrre.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikluklzf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hpkywnvu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ootcfogl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3upoourhv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3afbxuexo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qcdqqshw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cjsbxiuw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3shxglvsf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ggfllfds.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pupxxdrg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bilghdte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3huwidwud.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzfubye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mslufjya.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jfnvjmcj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3omfkpjov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kgamefek.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3roxbbexy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmpovvu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wogoqbdv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cxqzmcev.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hulnbhrw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuhsqgyf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yvcobvhu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wlgvsnes.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tlvvtsmg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3exvxrkoc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uzkvzhpk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ygqjsoit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ggpzljxe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bowwgfpi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qbiyrfre.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3stejrmih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkjknxm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxxzphuh.html


<!-- 参考信息 -->