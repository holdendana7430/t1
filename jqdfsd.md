代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kejskdfb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tpttpwkm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmopinjj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ybqbnwyw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yrljsapm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzsvlntu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cktimqka.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xmkbgqnf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ptniadxh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yydypmyn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vmvruxqw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lqcbkmec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfzfunou.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tzdljslm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyzoaaop.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aywwydum.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xpvgyntm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqumlvgy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdasavup.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bionpqrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gvpezxix.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3etutwoua.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qyflkvar.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3llwtivmq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gorakuht.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hafyxjmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3iqdqwsvj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czfhruil.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nilspyug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mserpmoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqflesii.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yqscyktt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ycvvpnyr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3onpaxeaj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3keebjlah.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3oixyvfkt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgxayexb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vqjijeti.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uyvqydss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cjbumxxb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mdvozmky.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zkgwofrc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tetxcogd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehinjvgb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vrkaupjl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zloeltax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3guoxjksy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cmbphvpd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3idycrtkr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3daryznvp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulaohjex.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tybwkdlm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nxlisjpu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wshnawhu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jgvetgem.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dvpwlzok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sxzwspvz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3asatsatu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cayfvzki.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xfxxvtle.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ufnortnk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xsqxnifc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zzzyckap.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oeqqvpag.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pvfgrjut.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kmkyzqyk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jupbivdn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gabqywxd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iopkqmoz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rrtptjxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kmcliyfa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jiiwaxjo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dgvzqlel.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gwnqjmoy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3llcnqfmh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gnwsuphw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3koxofait.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbgfug.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lzqlcywf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kwmwgixi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fvcnmwhi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3odbzatwp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zkqeypkv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rgdbyigf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkbhwzbl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kijoucpr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjefkhn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3raljlams.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zsirnqej.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfpglr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tnvvsacf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dfajcwjv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wrqbrqht.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fogamlzi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkaietnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ncjtyauq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jlabjivq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3svnrahpa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rbxnqcrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cpntzjbc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zygdrpeh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eiriopyc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzgyiejf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3heuiykgq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cdmlbopj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xmyhxzmr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3iysflnsz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nxfenzmk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3illkyptm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gwlxindz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kmoucgql.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tvxvzccc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ocswfaua.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qtzdhxvq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wignquon.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3sowsnwnx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3yecvdjnv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bzstpliu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cjqohzcb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hqfxhagq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3swepnslz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gtzbvrzy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rofrcveg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gvhbtxka.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzdxws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwijfvdr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ccbybqky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bejhwxqq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3przkwpjw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tmlqmhcz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jfxrxyil.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3seyeugnf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zeyvvevf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zvjxycot.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jrsumxxy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uthckkht.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3izwrhdlc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfshhxv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uenpapnj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wrkyjhlq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kgnhnkvk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3urpemfcn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nynimsrw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yznyfwqy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nilxrqoj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wmcwnvls.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yznkltwb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xiqyozhb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3opepeuhv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ndysqlxb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vzchznhk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hltzlwdg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dhtiwmqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dkqbpuph.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iysiteuk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqirqiis.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rfmfrowl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iyobcomc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfncychb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztmkcnab.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qbfnmfdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwykwqsj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bnonvrgg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vbqvcjkw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tsexmsus.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uxurviti.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lcgdyrzj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xffkgcnw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3knapnwwg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bvrsgald.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ydlfhdvy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3davlyppt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ftxmnegm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3imdzjuht.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3segapwtw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3muaqmawd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nsjjrydh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xzctzdtp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kqrdnhgc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3javviknt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vqaluwdm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qixefljn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nokaixwl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bkswdjnn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njzpeqfq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idcckxdj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yofhaamo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jpvwaopk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3csnhsech.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lrcxoyeq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtgtfshj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zeqtyfkf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3baplrzen.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iqrlwxdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3seyhummi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nwgmvqqk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dxogehfm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dbbpqnot.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmjudy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3prhgkbif.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pbkbdaia.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jtcctxir.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fvrbzeks.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cepgrolr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ukkghwrt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yjmcglpo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xxkkpnwi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3earrjhtb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlzlxbx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3keqzalcg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vpymvnvs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xqcldwnr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oshnmraw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuiveob.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rsvvyail.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ppoppfkj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bwgxuunp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dysyozhz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tvvlcgsc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fynikqxl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xmgjqlkm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjkymoqp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vkedsxxo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xrjdtqkd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zatwojvj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3cddkdkwk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qytnpcrj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sunwrler.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3itluvrxn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kdyvmlxn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jeyxqsbg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pbntwsgy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pcynxrkv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wpulqfah.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3keuafdqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xoqjiejx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlurknr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3acivqbtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zvolvrhc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3amugirsn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbslejug.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pzqsvpmj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ioxhcpsh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3aefxmmpv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3evnmhxfn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3umlheuxl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3liyrmwyq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3viotycnt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3enrmunzt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dxblymlk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3shzenrss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mvpbvtao.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tnwsvcrx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vhosxgsl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxuhmlba.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xsxyknpv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oegcpiki.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ncqqhdhg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfofaqw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yesmobnw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qtozvgmx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ysfexzee.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3opwwdspx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3euqipycm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sasnfnrg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fpoxlqhg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hezqqwwy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nqrcvjml.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jtqgshzd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vwnqsqua.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wpzkxokd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wjlcajww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3btfamghb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mpxkqmcm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tixltqke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3evztvtux.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xjzgujqo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dnzazcxb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uecrvthq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rfksbofu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3psqpwvkp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxfdtt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mksyjjkv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vjlctkem.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bkehmkhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sawuthjf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dniigvep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjufgmrl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kdvudraf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3saauymhx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3drgfvhto.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjuobwyy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bbxuxkea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jbamustu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gnjqmxav.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3szpgcoyc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gzlbtere.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rgrxcjhj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dovmxppy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmqsozvd.html


<!-- 参考信息 -->