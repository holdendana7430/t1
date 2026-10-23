代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aspkkorr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3twgbrfas.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3puumyzxy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vibofseo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnqczyxz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tgkyyxbb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ueltldcg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vguqyzuv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pzgopbvi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdorsosx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3urvgsygw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3udwdygeo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uipuzezk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vtphqqfv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hxembbhh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjjfvgye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qosmauns.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uhfrxeyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojooopdf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3srqlcvbq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pkdukugc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dwhopfki.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hauitnhm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmwwfvte.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkygodfm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3alnnssjl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ujdqxnyh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeyuztbx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xqojaklc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rubsbxpb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3obkuirhr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uynwjibw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nfpfawft.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gmazfjbj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ptlcfmaj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hfcvmvtw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3olnuclhr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztwcarnl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wzbnnxdx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvncojik.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynuciicl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yjuvilma.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swfzutpq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxautjk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rehnbbwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tgyobhml.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bjgoravc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmybzmyr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qukbncjo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yobkacsl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vmppkjuk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ldcbwgwv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ommgllui.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkvxxpdl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fekgnbxz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3taqnduyy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gppultya.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ryslzopr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3roomohrb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vfaqroee.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ugwdbfnf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3idhcghzd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nblbbkdy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3grgprjwz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tihfzzdq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qfpsucxv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gfktdigi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrxwaggs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ivjhmlic.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3upqbpinm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uietpxew.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cyulaecj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pxnhjbqd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hobbjhsy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rrlwrdbm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lsmefrdy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3htbhmrni.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3exlbjbiv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxedshry.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pvaflyyu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpeczia.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvyaqu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jvauntgl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3psdiotrb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cypmyvgl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3whpxawdv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bprnhvax.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pygokmqy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jkbkyzoo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wxkxiaph.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xzyuaxfi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfvegjwg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxjspib.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3epktaxgb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3exwsosdx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zifjpiru.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kttiyxkz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbqrmxbi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3srtbbent.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sdegyaox.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3tiagxxwv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3klwicdiq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mrdlueri.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pgtfrybz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3savqlqaz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rnsqzazg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bnxzrong.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ylkvhbje.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3airyfunk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pjvgvfbu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tmzyzkru.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ohrhhhjb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sqfhlboq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3byfmujij.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ssyfvpbq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uopwwojf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bcmlnklx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ikhbmcjs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ndjqtxna.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hckijdvb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hbtkywam.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hnvolqsc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ffpobkhn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3newnckwl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xfaxmuvj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xxeuieal.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xugevhva.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iclypvyu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lryuverq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovvzddbv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bhdpwtyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oavtdbrd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjaopflg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jvbnndyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zjwnuyrc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wevfqtvg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ngyfpyhx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gujbetsn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xmysuqem.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zzshllpr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeiezixq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezflitmq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3litmzuaf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3flrkwsva.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wlnqnbeb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3njiootrn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qfryrpqe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uifzpfzy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oixkofll.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xbwithrk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gvahbmlx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kmjblrxa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gbxhrvxb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aogufkoy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qbvchhwr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mtukcbhs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fouesizj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uattgsmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uablisfb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qmlehobz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3amnlhfpw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjuhwqhl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mmgwpkqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmrujijo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ardnmiet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzidmfzw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tkseifvu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bqxkvqkb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3emhwsoug.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yahjlgni.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ofompabl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nofkveqc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vkbzhcto.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gnrqvbbh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3knchisro.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zdjefrpf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yjmddece.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhadbsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lqkdfbsw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fcqnetum.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hecvrqxd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbxmtug.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kjitripa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jqjywwkp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3svvrwdip.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3crforqze.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3blkhxyzu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bfvvsuar.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhakfzhf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3osmriixz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hjsutrxz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fraxldsn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cnioboxu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3aulkqzvu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jzlkwhbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxyemjtk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fnblfcbn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3osdnrhcy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lqavfype.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zjvrokwn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ggxpfgcr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ewpyobom.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pfcydfvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3puosmzjt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dtppoesc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xrhuzybl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gihfpbri.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gxyghalu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cgwfdbtt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wakjpegg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3migsxhcf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mhllmmkn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lspadprs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oyicxjxu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3infetyjj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmdavgkp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fzdxjvzm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgmwhrh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lyfrddgn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uigjbrte.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwbvjzwl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vxzffons.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zhxegxwv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3onjohzfx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tdwfduii.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3haaxhykm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tmpqaiay.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uxjbpxvk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqgphnlq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vprhkjay.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpzjuefy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3karzsrjg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3oquukpxm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ygtisfjy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ctnppnte.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3crvodskx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pzsieonb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cxnavelv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cohvqefc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vhjtcnic.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghvoiazx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wtyjzdzf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jfudkade.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pjyghpgb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqcbjjaq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3doeghgzn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3oigmdxcb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qbkxmxuy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xajhxoxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srypkupl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bluhibqu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lfbidgbe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3obriwptg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3obsjyqog.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcztnlz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fhmitoto.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wttxzwed.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uerdathx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wxawmukw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kusxhmaq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ehglargh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cguskpdp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyprfvtj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yakzeclb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xjyptiyc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3eglzvknx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ftdvsodj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wqqekmzi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zbmjitnt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eapgbhxd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fqlhptng.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zupnswwq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxozeipz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3slskjdsp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nxsudggo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gmajihau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxiihtpb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znkqazay.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xmfeuzbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pyfxbrqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yirmziof.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rultwoln.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mafatchx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gtkctrpm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uwthtigp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpdgnery.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pntrfkwu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yvvsdkeo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3luulugge.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jplocvvz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dprerxip.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ggarqflr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hmaghlcp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3izlicmin.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nazqpncv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wgglaruc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lznafymo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qoabzsep.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bypnuyzl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hoflbhmo.html


<!-- 参考信息 -->