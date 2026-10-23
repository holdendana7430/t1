代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uilxhttp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ledkhqvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3nulvufdp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvaguil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sohxnryw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dazloqfb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umbrkcbe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpskfaty.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgdufljj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwrbvag.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3phxgcdnk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nqacysaq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xbqizwnz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cjxinmbh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eclxtffo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izecoour.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3txcvcwsj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iupxggus.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amlhsmlg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zsdtvftp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cfaayiys.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtcofrf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lynenhzw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qhmnduxb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ircvsyek.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqlftfp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ozcioxir.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hexgtvwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zadmghhr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3szvgxhwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taaoqdvk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aekkryak.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bxxxuotn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aikikdcl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzvppbrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbqvefkc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xdpwkepe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lczwrsdl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpzqsthr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuackglz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3azzehjaz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gugwptbz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xqqpkpgi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvrvlyp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3raidcogq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3okbnloes.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fprugrof.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3epgustev.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qvknjkzv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3obgcpiwr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cbikutcn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3onpaupii.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gzzpnryo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rglcfwpw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbadopuj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3brhhdrth.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xhjvsvsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nldotvzd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbquxy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gznglxtu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ekumzlan.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3touxetth.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fgfajsen.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ovyniznw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dyrulqkn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcffmgg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hjubotea.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xkgqhlsv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xjsjvygw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vjsisfew.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fakxpxwz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vujzuvhk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cuagyeaj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lrhjwfei.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3czinuaxk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rowjmvww.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wrhvxehh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3laiinkas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3azqkssvb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tkucevin.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3isjhjcui.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3outfcjgb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ihehafua.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3owsumvfo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dnuovtca.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3liirasyh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lkdlrgmh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3estwkffz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zcqfhpkz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3axadgtgq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ulmhwkpi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qnbtjffx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jbguexlj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lksmnjoh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cevkxbkg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3naslfuuo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jsydskku.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxwtjdn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeqndlun.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hlhdhphv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cndwgmks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3srsrbohr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgowivh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xucxayif.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qnomnvao.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mwbuaxmi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pqgdjnry.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3oeezfebw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxaesrl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eeciulkc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lvptucsw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rrtykuwo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ymbdzoxk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zrvtafgi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hutsewkp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hlrcavep.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qiokqggb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eszwjdsk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kjdfewie.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yfhltktd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aoekvcgm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3efovfkpg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3emzsmamh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3auvmeehj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ggsgjzow.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3brnozxev.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qzccqvws.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iydpnnky.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vvyfobnb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fpojsvjh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nyxtmxif.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pjgdjvcz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3seewhqam.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hnexifkx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kgjavmav.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zxowiimc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ubctnxwu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lvkwbtnz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sudydcig.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qdlizkyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eayhllzf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lnfvbwur.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jzzwtdfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnrirckz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hzvdvsgj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zeeviaak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3slvbedge.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yusiegnf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3givpeccu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kncodyuz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ctrysace.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jfsqyphc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfabrvpq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zrgljzni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nbcvlpjt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3frxqtyea.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kgiixegh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzgekhdh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zpkfmyuz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hzgfgitm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlpkqaqo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjnftyqk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zttwcusg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oxvgcffk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wmjojizb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jnvfrgcu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3knsniuwj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gaozrffa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3glkafwbx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3swedbdfw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vahisixa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okpxgtke.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dyuvfump.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dshcureh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jateiarn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpmdejyq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sjjatxvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bniwamqe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vilkvshp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ztbeuhgr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dpcabplz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sohijukj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3snxgzmge.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rfoiwpbg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3svnvfixj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fpdrgmgq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxgivi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3lmyojubf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zumzdbnw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3twgpjcqs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ruwclgpz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjdjdvlw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3minafloa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtirpdu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3drvvygna.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ryyvhggh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ldkfxjyj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhjvepg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rqlxnnlc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xermadkr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjqzbbyi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eprnehfb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dmmkqots.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kjcbhygs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsodxncg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cpzendxt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ecnlrazj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhiiefwz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3iveerbra.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fwqsvypw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xylaxmnm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iprjtrnf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ohohubqj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ktjdawpq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jbumkrre.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aqvezean.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbifmczc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pevogidj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3enumiizu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vcokucqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wucbuhsd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vrtcyhca.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lbeqqrkf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wrrkksjy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wogfpzpb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mybjymuj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fpqravcj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gcggqnso.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ooarfopf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxxgcsh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nmtgzjcf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hhqdzhjq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3byomryse.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vzjjvjtf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tuvflyjh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3axphuiky.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgsyqay.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lkzlnsxx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fdpodfod.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rznuaapl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oqmjdpmm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rljhvqoa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rplcqcuk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3guwsqjyt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yznerrdm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xloyevdl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nxvydjcr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zznnflmd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3flclyfou.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gpuobpwl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hmulkjtc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wabamwkj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdjxrola.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oirkapjq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ljmvuuuz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jtdvfchx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eplwarng.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3avicgdxk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pppmzokj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dssuzxnh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pedxtwln.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tmkshers.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvyydym.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwwnjrp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3iqdnqqiq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3atoojlya.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cigqldzf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fyskunol.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lpjeqfgr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rdlhjies.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lcueanqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xsslgjma.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yfdstnii.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rhovjnsz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gejceqsx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hwuhyjlf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xjpkjrcq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lfvkeiyf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nmreklmd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dlmdzryb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zjsvpbkx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uftgesdu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rjbnpupi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3scndtyqh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3diviajug.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qlfnsglh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kwfkmngm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dmzacomm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ztogbrfx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ynyqfraf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzygefb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lyqdoxkz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jnuqhpgw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzgvnxxh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fgppmbsd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qitylctm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3acdyszqt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avdtkobv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3acejcsbz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3turvuuxf.html


<!-- 参考信息 -->