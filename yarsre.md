代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmutkesi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hhqmeqhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfhkphtd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgeahfen.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uzvbbuvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfuymjkh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ougtjfem.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwqbgxxf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyezxaax.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3isavkdtw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qkpqzdks.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ezagdiar.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hbmitlvi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3byipxxrg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfskfayb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bympjwfj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cgputrps.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cjdjavab.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lntltizs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ewyndnij.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kgsdvavy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gqqjjwbq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3moipcaqm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrxkiav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvozlpow.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3svmquapa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dunboboa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yhxhuitq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zexugzlg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rxlkfeji.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ucaccxzh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqxjmbo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xusogfnh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dxctyyiq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tkxxegnz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hupwkxng.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hpzykmte.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pgdmgmvd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzlsbpx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nirbmmre.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mwqflpgx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aykjbiny.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pntlntdx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cowgkrjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cqblxobm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ekbzvzte.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pstsiukl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zanvreqn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3udhwxkci.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xmqswwig.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3igmvqxtb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3grwgiupz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vkmymzxu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rurlhqnr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3udtnznzy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vmcmofie.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ynaaljep.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zioexhqs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cxlywpis.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oozlrdqx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrrwpnr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ognrbpjr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hndmuwal.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jokciubo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwnasxg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rqqneoxa.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fcbgnkeu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tqumjiev.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3amzfeppq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fayinmux.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcgkrydc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bdsojfha.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nqcrnpdb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3timfsmot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3njyrybvd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bymrmxil.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwuyhoj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwgiuye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rkwbcivt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3omnepilg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mrsnbfme.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xldbhtxe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kasmvaga.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nnjarzwt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dyldxaxi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3agjwlvkg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pamczivc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gkoraecj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hwsgtuel.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rtuagdje.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3merpooqq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3axdshljo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jkjdvmzn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3enfphusz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lggaynsr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dbmarxhe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vjujyubg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vwxiqyrs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rhdbired.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gdajdujv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3iqzjvsqc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gusdlpum.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zfcgvsot.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qvcxulsk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uycpzjwu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ukjlqdlh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3isaqfiav.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gdfikbzh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkshpf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3yvugkhvx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ltkpjudq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vtkzztzu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zvhrrqtw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qdimcsrk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rrlkmiyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bcwgkzup.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jchvqyvk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uktzgnxh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dkglumww.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hywjjbmj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uvcrkyfn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3uehiajin.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ialjfual.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3orcuopsg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efscyknx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3swlrlptk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxixivl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dbiwpoku.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kfeoihqa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrjhcqyl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wnaniqzc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xyhhbvdq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekwxbphs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xjndjnng.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ruwebeou.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hsyvuotr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gwsvbxip.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sbllgxyt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yglptdwi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gvwfxeck.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ndncbpou.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wezcsqqe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3veelluzt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcboucwi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3icojbnhj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvecsb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sxdlimia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqjenuqw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yckrrpei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdoowsbn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ijzagbig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lcvxxwox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xtmwqahr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3npnrufub.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wjunrrka.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dkklbuuq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bvrloxhy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ngcixzww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3scehtqlr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vvnivdzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uofzepwt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zdfhmyeb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wwbxfkmt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uojidpeg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mqbbkkpn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xnlbutln.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hhrjlfpe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mfzxpzxn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3eywkgqdj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbgvozsl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rwicgkad.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gfevdfhu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wruxwghz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3orsfvktq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3orqnkgoo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hetldrqu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ogvdrdhu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bnstrerz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmthrlic.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yslluklp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bvjakwdw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ewyzssxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gimtxcrl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xvpeozgq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqofausc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kmvxysrd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nxwiufyu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3axrqvotc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rnqpwwhf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mldmxlaf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wmlkzrur.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3swargbub.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xrjnslie.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cyikeaat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3szqppose.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjuujgqq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzennvoa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gxebxudm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kcdhmtsn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3girrcdri.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qnxumiux.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uaupdsjm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bkpjygdk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fwohcmka.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gqioiwth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3udpzmazg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3arurtdwl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhxebcyv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zpdczuyn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3glwebcrd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3oolzjtda.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jgnzrlrp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqludfne.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3boccbcuw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3adhspxqw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vmwqzaca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kfmklprf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ketfhbfu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ohvxujxb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3szjmcllp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzoetzuu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hhzxmwyi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3odfrvksb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jufexoye.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3plgnvziv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3eiezwzwu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3uzgyfiet.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dmtxhkpd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lxyhytos.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aymiuazv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nwvyggim.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3anaywprj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pprvygrj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mnhmoxnm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ovqyijjw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3udkgltmw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gqiyrrvx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xelfxjmt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3exiaostz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3sqsjsjdl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cooeaqpb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3khrnidga.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rhvcrvvl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wurtbgxm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mmmpxawy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tzddnbfc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3swatutso.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jopprjts.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nmgciryu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kiseukgi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3svnvcgwd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgnfdcq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmsezwan.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yuknqoty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tttcmrga.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlaqkzv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgufawqz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmdhukf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gmgncliw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ggohjhnv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fpapkjnr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ykmeqmgq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wvmrywml.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wuzodkch.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xqzzdded.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gwudthlk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkrjvnzx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zwcxiixh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3maratsnd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ebigpgub.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxozljk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qazqeqre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkwwazg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tdzgtiio.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pwsrfaws.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rziryabi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tylwxdct.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rmfcyvcf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sbdskqvv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mzrnwsir.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qwuillgr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lsrtfbkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uxgmkbji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wndosiue.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsappsmm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3blcibovs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3taoqoucp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lismhnmn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rxbvwegx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eshozixb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3shhulbow.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3npnkzenl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mkxxjoga.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lyzrxltq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xzrolhvv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyjxuosz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxxgwqe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihazgjye.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkjuqzae.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qrjfapem.html


<!-- 参考信息 -->