代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qaibyczh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elvaljvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzdjgjh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yqjecght.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3acnaqens.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xifcrvhp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fqzmexpn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dbvubcoc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yvtigdfd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ritixgur.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hnaztfxo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mwgwprje.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwidgybm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3quhqptbo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iripfryo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3diksnuce.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqzssazh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3blumhsat.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tbrhmbtl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ecxbmunh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxcrerh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3smogricd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ricfryvr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qqbcdxoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrchayxq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ynpiauun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oswqqrom.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yleoqupu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ysehiigq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ahloygth.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeooxcoi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ysbsbmrh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rtjcrejg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gonbtwvc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mljvleuq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtnettcl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dsarbyal.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lxynlhbn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zlltjjlc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3clojjanz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfeshebw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yankarrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvrokgmy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kmhkdqck.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3svedvzmy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwtfxeqy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wzjvxwwz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsiwycte.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3awynswts.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kksaneam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdqjnpl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdjmsz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3futijahv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tambrisv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3liuewhdd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtlnrhh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vjczyckw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfvjnrww.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rekwuxtx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gvbepges.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bcidgcvg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgybzer.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cpnjctir.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uwbpshwl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3agxgvwvi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3icdzeodr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3euukkeyj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cjuysakb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mtyommfu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hgoolgvv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nrmsnarb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rbglmslm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3khvvjskm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jrxwevsv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ooamojmm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txpodibn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ycpvfygs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bljmngqn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zacplmwq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3omyniqkv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3udnkulws.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rnfbeakm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lpellubq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ymvjbqdp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wnebndph.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gschmite.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jgwmaosx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lvczcrtm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3amrnoydk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jzowidoz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qsugfrnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3piopzqvc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yeckfkch.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rscwhhan.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uildqgww.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vfatpklj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wipilfde.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wisewafq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yzroaabs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uxhxwqeo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmfymvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogvfsowv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lyhoikrj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yafyohpg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmelmmi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgcvlnzp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nprpxeze.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rrofbosu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3alzwvttb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pnrifngg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ivpdamnc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nviueddv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3blvgjjla.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ljbvvlbw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vpvvqfmu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jtuqibpf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vqbtvjlp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gcsgjbtg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xxmhfqef.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lpvhzrva.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3toeuwlli.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sfzgugwf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3znnlwezy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ncxvpfeu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mzndxzne.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vnfombpf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eqbyiqmn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3iuctvgyo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pkhpiree.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3viibugck.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3egwijwwy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jvubxzox.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uwptdhho.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fntkwzzo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfyadbpq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qwowptss.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gfomrnyi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvuazsy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3opgljapn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3datohgsq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzqgttnz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3abjypknk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fwctjcni.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jewlykro.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnfangps.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yocgybzs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3imtddfod.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mncmxfsi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfuacnsa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zfmqitkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hvlqhisc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mgcqrfbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3krwnhnpf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ptxxmtxx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xmszglcr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lkbvpale.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lrswahtj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrwhslnl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gvwwhhsm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vmtetigv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ebvxrsxp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3adpdxrmm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uxnvkrwm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3szmqqfqa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hibwtbyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3eklsmjec.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lmdwyjmv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aabhryve.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tpxteuyl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vqojqwnn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jqqcywyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zopdqvjf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vyphkaxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxilxyjg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dhodexbz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bvievbls.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wtnjzqfp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3etufehzd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uzbqbtcw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iufdqrvp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fsryzhyo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3azidhifq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tcwalsrz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lyhebhqm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ccmxrwhm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3oakepodn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3agpnlwte.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3reslqlul.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ywyjgrsw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ixocgxbw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3slducldf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3atlxatsq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vbdzikef.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gflswrhm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nutpaspa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hkhvhxly.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvmwzyjh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fpacqokd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dqyeounl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wmrmqbkt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ywopcsel.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mfoczwnz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzlfafpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjfxcnde.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nndflepa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rbpwbnnt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fgbwutmw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3firvrwjc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcrssvp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vhbkeuew.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jwcoiguu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3grazfbgu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcdjxg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gnnhyqvt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ukukbgmc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3esgtcjpe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bbopyxgn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yzuytlnj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zznoicvb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uaqutjgv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhgdkgfv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3asiranup.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3psedxjjr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mkgfeyvj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tjkvdwpc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxijrtkd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jwcaiacf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fjpfyyhs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3stthinaj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jicmtvdw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tmxauwmd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3euevssec.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hwghquzp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufnyszoq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3exkdumlt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3czzqndjm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xplixqyq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lyaqpkdu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3sdycccab.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zwuunqil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dgupqcgc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tyjxvwpp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfesvnol.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mwnugflc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gagyhbsj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixbesgtu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ytwrobil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xixlqlca.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mywkplmz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3urpietwe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rppxlsts.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pzglovac.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sgzcxcvj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qyuvrciv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qskukgdo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3epdbktne.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iuywvxwy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3guataeio.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3afaxkdom.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wiwoejaf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3whqeaeca.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sgleujvc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kqrqcndt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ehghidsx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mmrtzktx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vxdwulfx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcdkhyqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cnlpgrdu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pyabrnco.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3seswfsvw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vipgucof.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gtnccjbf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oljmffrx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cvvheiny.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ffwncyal.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vbcetyee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjygurj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gkaeufjm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3werlkwnb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hnxkpors.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jzezsqey.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wctkrtsm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fvtiuwrr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3htrlvlez.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nmicsrui.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pgirifrn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3idquzbks.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3askqzndu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xwsmdmup.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxtvvly.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bampkixj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jpjgawhp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3behfzaia.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vwomrdfx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dheieuso.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyoaxkky.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ozeutxhx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3imupffgm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hddhsllu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cntrzsyd.html


<!-- 参考信息 -->