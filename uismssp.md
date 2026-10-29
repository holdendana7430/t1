代发 wailian999

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwwjdaeio.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gjrfiadua.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gccqztyfw.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gwtssybbp.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gxaqeuwln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gobpbbbwr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggxmtoyjq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxpizzkik.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjncbsxru.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/guzyexeoi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gwbmkkvhz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmwfnslqq.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gwogwnyzk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gtitgxbez.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/glreiyuho.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbizgwxeo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmslyvrem.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gdrfcicwc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gtihetvzi.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gjqbdbfem.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/ghziunztc.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gjiglmxtz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gcfdxatlj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gebgsmudh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gldpmnuzo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gmqzggjtn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gxptvvcgy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gswqwkgcb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/glqozbjwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gwiptjawi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gqirojymi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/goyvtwmue.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gqgjprqlp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gjcdrfuqf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/goyzccftu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gwbopbpsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gwprrbpvt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmfvddivp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gxssohvbn.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gleipevyh.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gvoalyrcc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gsqaxrnok.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gshgedsvz.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gnynszlkn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/ghcfpikiu.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdafkszfs.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/glvyvvljp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gopvmzntw.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gmbagtvah.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gojzdvcxr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/ghjpkbgtm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gzqaxgoke.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gejwxgcrk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/ggprqnbxf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gbeldazwy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gthcfedna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwuazeefy.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gjpapeuce.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gwyzeyqws.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/ghpixryai.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/grlgwxwtf.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gmbvtobfx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbaaresyl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gcvgntfct.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gjoqmdsqh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gallgsnja.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gqjcoknvi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gyzincdoe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gbcmlswqk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ghuuiklox.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdkhpbzbu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbemtfcte.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gnzxhqclc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gesamkcok.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gyetminhx.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gmvohpurr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/glxtuhcor.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gejghgzyk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gytmgzlvm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gtvqgblis.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gjqkzunlh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gabfuvbvv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gburdtuoy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gusanzdej.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gaianetfu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/goamyhyzo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gdzikxgtk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gtariclfz.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gnhxnlczp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmewmtpoz.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gsxbmvuei.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gfhnfghke.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gelqszyrk.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/giqofpaoe.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gvawkzswq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gtygsmpwj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gjftesbuw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gbejmsdeg.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gnptvvnez.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gchurbyvf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gvhfveeee.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gyxjmdplb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gpczytkel.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gkauubydz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gliegvrwb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gmeuzvlvw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gsmzsyrss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gpuewlzwb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/geknoiajv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gwbyarytb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkigixecb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gavqcricg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gokaysuur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gessfacwv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gqysarcvu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfcexskvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwueehfqy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gdmhhvymp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gjdavvibf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gaqwtefgw.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gvmsrslww.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gxbaxnhqr.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gcdhmlmff.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gwopdifff.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrouphwj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gjtlntiig.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gvpzlbbzd.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gwporpjqs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gpsrvpmuf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gnfsbyhey.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gcklwpnpl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gvxbqhazl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gszmhyrhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxjzhlwpx.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gtlrsrgsa.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gmiimjqes.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gpvughahy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gmuguewwv.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gxybduzdp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gwhrlkrdb.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gnqmuqkxl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gnkyehvgw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gwwybprxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/ghtxooxvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gdwvadijw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gpnghgrdq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gvhjhnvuf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glluijabv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gukozkfyo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guzwptyxq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gowehnbso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gcahuymds.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gqgeckqeq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gzkcgwyay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/grahmghxb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gxmopcjxf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gwglkyjbd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gyhptvhqj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gbztnoaqa.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grwjhaiuc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gdtjxblkm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gjlouikxx.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/goubhuqoa.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gtzqzpkzc.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/giafuiwrj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/glsymfdxw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gsksgywtr.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gzxhdblxe.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gpmrewpqb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gvklparrx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/genxsqbkh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/glasdcvau.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gywqitdwu.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjaxogdgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gvwgpafbb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gsakxmzwp.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/giyzucvbb.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gxbkexrpm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gqxwegbvd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ggljlrjuu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjfjauinx.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/giitmgarb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gdykyllvd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gnbrvgqid.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gwatquiri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gtcrcmajb.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/guoonkznk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbbnerdqf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gbyemerop.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwugqzybx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/giqcjvwcz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gzudearyy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfprrshwk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdgoukast.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gkbyrplhh.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gogvuvysz.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ghtoadlxf.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gnnistpdc.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/grmrcnzbl.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gbbgtcudr.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gewqjucoj.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvmhswuim.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/galvbzekc.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gfkghtpfu.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gztvddnlm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gyflujnpf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzigjrzxz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gsieitufy.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/golytoetb.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqsdbjuit.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gazeikvmy.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gzkticcxu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjlirnuew.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/guuibsbwv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gatzimcmk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gzngjembg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/ggmwvqmyj.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqbkwseam.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gxpkgozzl.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ggwfoahfl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/greadsphe.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gwnsjpluf.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/grcmihnam.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gbqfakyiu.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvqfcocmf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gvimsymce.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gicoqppna.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/glvvbtawf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gelwimrsp.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/getvvlndw.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gmppniqqt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gtaaqqxei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gikyghdkl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggfyrqpfu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gswyhtnoz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/glfzkbrsj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gjfmeaobf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gwcbfeazm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gpvaqfnqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gmltofvxx.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gmfqelxdn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gwkgkcskj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gvxrfukrn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gnazqjuol.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gqibcxucm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gfbekfget.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gxnbamsds.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gwjzufsbw.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gbfzbqhbp.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gghewlygl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gqauezfcm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gdczturam.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gifofesht.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/giajtgvmh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gyhwedbkn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghixjvjrn.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gipzlzokn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/grybhnxlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gghjadltb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gpcbgredp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gogzolfbp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gthrinukb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnqmiaevq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/guhvfxcrm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/grvfycqex.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/ghvcrlgzl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjhknmrpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gugmskhck.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/guihwrcbj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/grcvlcprt.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmjqxtbgi.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gawusgwqh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gejtmhesm.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvgctchyp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gktlcccrg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gqgrboonu.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyfevsswp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gmfxazbin.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjtlwkvfm.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gnkrdbvvq.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbudeuwrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gfmggqrpt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gerlqmbgb.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gjeobpsnw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxffynurq.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gxffhjzrb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gqogvonnh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzlcmbmlx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjkoxtzzg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaedefafu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gisocvlub.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gwwznvofi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gsddjecdk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/ggkmqahcl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjqqalcvu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcchgpszj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/ghhvovawl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gvjmnpdpd.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gnzindjet.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gnbzxxtrc.sHtML


<!-- 参考信息 -->