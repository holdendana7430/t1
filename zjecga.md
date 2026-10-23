代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bbnocoit.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3stksxzfw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lrxlojbu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vlkfreiq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3serxgoul.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cjxvklbr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jemxwwws.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gesrvdcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgmrlovp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3roboheam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzxpkvod.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jqyuujdt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3phhfjbhj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxnhofmr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdwaxon.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixcqrsmt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvvfchm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pqmwjgip.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jeatqbfp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yobrwyvm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3plcqxuic.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nmycwhae.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ajcmuqzd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3matwwkqp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pmsuxbuy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bfvydgjm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkrhpntt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xufdxpiw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vxkhklgn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lanwviyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qnqewvxt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tfcxillj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oddfiqug.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dbpheprq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ilkwskda.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ncydcfvp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhfiethp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ubmsjtts.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygubcfcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdnapgf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ovtgaspn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lztndfwt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fxqylwse.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zgounepy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zywayzkk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qdpyctqy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gplalysy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wueznfea.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3phtgtpid.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pilkpyae.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jvnlqzoy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nlxxiokd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rsgwqlez.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bmsnktqy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jgenlrzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3snednzik.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ahfefnei.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3whpkcylj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ycyxfetv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pgtavywh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kinavalj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wzeemdzf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3omzpiets.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nbnpvusg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3apqpotht.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bfanivpf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wphxuopb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwafsdco.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3btcrrxmq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrldmhu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wherhipj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xnobjfbw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mehrffko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uryhiebc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3cqyoaktz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kgjpvezb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3iukskiww.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lttjzefn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpgjrxjm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mdirsapt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xpgwwjov.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzckpdpk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjstjda.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3evsarvxq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xucxzhxe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypiiikub.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wlmwicwc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3muwlyaty.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjgamktk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ozoecrpj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdmahuq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhnafqw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yjuzlmlz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nzgdwstf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xmgxgaze.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rzzbzxke.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3adjctjiy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nubiwpll.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3szgjzdyo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3diykdqzr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zwavvnwx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3drvrqksp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vdbqzrhf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fwankxhx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uvwuyoqk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dbjcuejj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kxeszmmo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wtzuthmh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rjwrgkzv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uzmcxdek.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nbphzcmx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dozywldp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkuhzy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3noehfhoe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tdtgqbjd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lvtlzptt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ntrrepzr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gglnqvbf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hwobxsus.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dxebkqkw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ptrxorgp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bboolzub.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xipymjsg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbwwkhhc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nojeakwq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eetqlnmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ibmlxwth.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nusjzxfc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qcntduhc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lomdtedh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xhbldmmi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bqdblfxe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qgyleoel.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zececaja.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtkglyd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lruptujs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3exbccnzn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjjttfyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3adzffvoj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rnijfllz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prsslrgu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjathxos.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ucukdmku.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iztsrler.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jflwphwt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fyaytzum.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rwjvbzud.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3akiwhzts.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dleavbun.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mtopkjkk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xamlqqqi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukibsswt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wstarfks.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3udruuefp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3smdjlzrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaftawjv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3syykmkhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdxxxidf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkjqkojc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hqdqbnaw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3blqaybef.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vqqbhobp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zaglgchd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jscxewkf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jjdchnys.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3krpkmyyg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pgmdelyy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iwlgefsi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ripprgkx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3akdgwdfu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gomvatya.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhixgfwm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqkrrbms.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uywryniq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wjrizprj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvsbrc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fxdcpxen.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlikzdq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3brlsxhgs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3nbwvurat.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3povibvdy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gdzucbos.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gpmjizjp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjwvaqi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hmseylyx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sxjhjvao.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sdztekth.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fswflaur.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bkrngyne.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3terafhsm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jumfgskr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gddkweeb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bltcuzrd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3iezzevhi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lpeeidrp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ssjqjjvu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wvbsdrpg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ixohoxzq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3akeqozow.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zonevupp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lpyhtzxu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gdxonrxj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wxbdqutr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wukforaa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekeamdsx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udcdcsjg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jxajyldx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uikgxaab.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fbfelsnl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtbbeqrt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rguwjfoj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qsyzdbfq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xsdrotny.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wzlvbbmm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qusoqlvm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vrjdagjn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3soptadww.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3buipbttx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aqlvplna.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yrcnrkiz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfpugc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdhmpsbu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zijyvgdp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zapolxbs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tlhfxkze.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3scdpdonm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jgzepbyj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xmfwgdxb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynuvynzt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pddurrzk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dhljseue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iqaforsl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rimtllno.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3chskhiqr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pcfqwnul.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kyejrjsb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxaihqac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lkxuqpqp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wunoqrzw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cpleadlo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cogiqcnj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xqwqvqfr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wltokgxt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lujqvozz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hwqvxzec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lwsfeevm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oruedyce.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jnljddzh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kkhpmyoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bhojueqg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fvbxxowh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3sqzdxtnr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mlxwgtbt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wpdpgmqk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lebdtmmw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xcqsusym.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ppihicqq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fyqqmcxe.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3abwuqcwl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zmcprobo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upziiwfr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qglpdswz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wpdfaram.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bhbesaoc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aletujez.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jvxhmvsp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gepzoxla.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bcpupyiq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kjgtfobo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iarqhwcu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvplvpb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hayibmyp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qzmbxqih.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3etxbemwt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cofqjxjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cznpwuld.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3omjsaymw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oibpefyj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dctdnzjy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fxujulom.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ussppdvk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovgwcvsv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gowjoskk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyrgagwy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fjoqppta.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3thxccpue.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fmlwmccr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qottelbz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wozivfbc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kbjvrjir.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yjewjksf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3apmsqfbr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqrzmffd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pmhfrmkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ccuxeomq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fvcqvpcf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phrxwstd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yabsreuj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3snqctbfv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3opzghtlx.html


<!-- 参考信息 -->