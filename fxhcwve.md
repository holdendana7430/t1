代发 wailian999

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gyermuqjm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gukfsukah.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/griansqtn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gqfsehsor.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvzpsocbv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gzhkaieik.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gckzxixxy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcmdgbjjn.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gimqfvkft.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/glrwuzonm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/ghobqjwjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjwvbndux.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvkkyvxvs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/grmxezyix.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gakvrytrw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gtfppuozv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gwhrqqbbw.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gmgdqlctp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gbpxzcrot.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gnpoxjiur.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gfnvhppog.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gmwhwouge.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/guntahayd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gocomeaik.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gicndfuwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/guacyfmgb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gforttvvm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/guxjlbwqy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gtvoympyv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/glmnxmgxn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/geqfppfer.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gdzgndudl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gcqvkhxyv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gdxekrlkk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbsooiyzu.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gnlysindr.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnhgvheby.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/goyhydwac.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gcihdslbi.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/goeccasjs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gikqbpqqk.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvhsvkutu.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gsdooahci.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/glbjorlvl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gwgqvecfn.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gultjxfnr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gwznfppbc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gakbxfwkx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gwlrjnpes.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/garjateyb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gtvoplyqw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gdyvfqqoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gyttjvwap.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gwjncwuyi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gbnsdcbti.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gamwlnjgx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gbxmuzqsj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gpunyhmnn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkutaoavw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gtykraijd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gvdiwmaiy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gotjhotuy.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gdqxdeutm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gvchkpbcq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gjphwjemn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gfutxqzuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/glbnxwrio.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gazqnzmar.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gzrnyowei.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gabcmgmqr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gietonrxy.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gkswmwefe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gnwyndgjp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gteznlmeu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gkuygdjak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gqqolcrji.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gdtzbfzdk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gyelhibjk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gzcibynjx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/grpeuhsct.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gpuilpceg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/goddguikw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gkrkzncvv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gvvpzqnqm.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsjixnseo.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/giqgoupzo.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gtthgaara.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gommsiuby.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gvuqgutca.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/ggjscksbj.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gdgrtxzeh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/glyhhvhne.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gxctuaudp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gxydjccgm.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/ghbfviccc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/ggzblgltx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gqlfrizzn.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gfnztcxwu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gnyvdvnju.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gsndasmyi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gcqvruilj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gbxrtucmz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gwnkejtaa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/ggpfsezdr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/grsjfzuyd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gxsmudgod.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gviwfptrd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gpmzuwdwd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gflkhalir.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfpuwqwna.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gwonbtisw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grhxfojfu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gicdldqby.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gowsbzzvm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gatjxsubm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/giztatseb.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/glgwtelxg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/glxezdjoy.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gouvgbvsf.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghukechoi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/giwndldxf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gaxjkkcfu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gsejrkhtw.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gthocznuj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gtsymtcsd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/goaqprcnb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gxlmlwnit.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gzxqkeghd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gjjrdrvyl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gtwvzktho.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/ghozwulro.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gujumwciu.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gtcmaioed.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gtmbsrnyj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gamrsuswg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ghyishzwf.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gnurjorrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gfycjrntq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/grlxfqxyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqychaglj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gfsyzkxqj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/giiyajihx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxefjndfz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goudgyfus.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gcrbotszq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqhjhudld.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gccktwbgv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gdfcmjhsx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gpbgvtekv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gmcjmyjdf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gbtlyecas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/grzkbjosg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gwjvatbsn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gbcdzxmlc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gflgoirqj.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/glsjtchzc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gjbfllquz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gxvchqwgh.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gldshsmbp.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gnnjcuomx.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gdfhkhgrp.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gayqmhtul.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gkdrjzira.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gltkywbng.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gaaxjiaxq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkwdzcwkc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gjynnlhie.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gnpybuelg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gnusrddsy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtkcqbdec.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/grpbvudqj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gvccednqk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gnektupnl.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gqgpcmsdn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdlegrtvn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gbxxjrsep.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gdcehhtcs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gtrdsatov.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gisiikpay.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gmpzlcwxu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/geiewosav.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/guzjoweab.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gurfcqtoj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/glsvoxcdm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvyqrctli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gofjlnxky.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gqqytxvuh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gtudbedik.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghuwmdheb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gxjibzqbl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/geeslxbxl.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gducjyhso.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvaxmojyd.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggxygrcfa.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gsbopvlmd.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gsutswwhg.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/golqqshrk.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gysdceikd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gjeaobvyr.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gnlypngro.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gvhdwpjvb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gfuzworpb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gbhssjddx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gfoftualx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gperhhdkl.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gshpbbpzo.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gzwssgewm.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gvjkobxlj.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gvofrejwd.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/glwnxubhq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gymsdcwiv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/geaifjmui.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gggefjskm.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gfucdfmgf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gvwptxxou.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrtavgdv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/guowddwpm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghadzmoeb.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gtkkxptue.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/geaawwobn.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gvlxmpymx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gcblwwanr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gkoceilvj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gmobvzaxe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gncpuxxwn.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gabnectgb.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gvdmhhiuj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gqpdxgwky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gkwdqooxk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gjbaajdfg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ghqwclgbn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gkimoalle.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gpesuwrqu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gsizsyeed.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/grmlqmnjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gcizinrlm.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gyxgcysmu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gikyyardr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gqupgnump.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gmitscdgk.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gyczzntiz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gajreugjb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gtuykmadr.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gzulktsgz.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gycnsautl.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gdrnupsxk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/grjgjcfpd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gslnwamwv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqcfojuwp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gpfdivgiu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gyywkfewz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvpthnwez.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gvibryrqz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gmvvqgmnv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gtofhuftg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggenkbihd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gsggzppqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gcybyeijr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gkixmtpjp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gjahypdko.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gdinppdxp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gswmmewpm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gebzurmov.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gmzvxmurt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gnhfuhotf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gcaovhife.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gmuizvdwi.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gdmsslvna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gvrxmobim.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gvdnofnzi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grupzbbzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghosgiejw.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gcfljthbj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gzwipdufz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmcziskng.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gcjibfzwi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmlfdntgy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gtpnshqjc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/ghwvlqgwk.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/giderdedd.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gedkhhmnm.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdnlhhcln.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gjykafriz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gkmolthly.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gbunjbuqb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gieqfbuwt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/ggugrrwua.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/grglaoxqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gurerfiha.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/goaeuthty.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gmhjwrtun.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gbyqjpgsg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gdtjnbthg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gmxhecrsn.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gtjbzymic.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkdityk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gpxjmmfps.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gnforosir.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gpicorolp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gglgqegix.sHtML


<!-- 参考信息 -->