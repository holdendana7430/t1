代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ghftmcxi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nzydisjs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3csakfrwa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjxlajtj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cllpvxuo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bdqkcqtd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3exbdactt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zzjpqdda.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zgpwqtyn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zkesiiwr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ipygerxn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zdmwcqbk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnyqegm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gutnogzx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chogzjoh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qlxjtkkl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmbhyte.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuggiarv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qosccdey.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zysusodo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gjikytlw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iexhdkvz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sdxzhcwf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nmpdusda.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wslmhiyu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hfbzmxtn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3editlmmt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wqkbhynh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nzdqiicb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3swcydjwe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tohfuoew.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gantrtjg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qnvztalx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lfmnvjpe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vnkyvpka.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pbtvtcgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdjismit.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rlubbtkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbpbwjvb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zppuuzop.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3moehohyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uvrdglpr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxdylvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwcsxfmt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkneefa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dlzlnthl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3easfiopv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyeuwuct.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ykbjtami.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3aynwlvou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpfymqys.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3quqsgovb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvqizlub.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zfpksgix.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hyrcckwg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3idlniond.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bbhznfmc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ervnnqgp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dljuwkii.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gudbycyq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfszfdp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3spvfldbf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3voawurek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nlsgplel.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xsupklih.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mrebmygp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdydazpz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gewmlecq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fdgdgrun.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aunllugl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3izcmoymc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ntroneog.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqepbxyc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuezylsq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hholsmzp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xfuqbdvk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3albptlnf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nglvkyqt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rcfhacev.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ewujxfwl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3aualvegn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qcvqvhcw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3woairtcw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pnbtcece.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wsgdoiic.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xicpcunh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rqobtzsa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydneinba.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pwkjqtgb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qwdoewnu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tburddld.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3othziaym.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfjtkir.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zkdibfce.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdnvhan.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqoaihew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gimaoxkp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tvpxyqsf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ootrkpeg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wnrwszul.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jeivvhdm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mfdufvls.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3allbecaw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3quoopxcy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqptvda.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkzbvbyz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgvtrzit.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yieciloo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwczkklq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddhgeogs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhwvtyj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ficauoiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wbjmxkki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohruijvp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iobxiqap.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dqyvfdrv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bghwwxbm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlespqca.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjgkoae.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3anocpbxs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uxstneor.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ofslazoq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nydmucme.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psjdfuii.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ukdfckio.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tmqrqwap.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jtaqoljt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yieykxkw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fvetbxvp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pbhmraas.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hsfbmdfv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ltkptnts.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3obyqtlpe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3aszucqja.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zyapxkcz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xntyrrys.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aavlvrtv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzalxa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jkcpgibt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3klsfaabi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xsadrgqg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qjmtdiif.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ioqfpxin.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ljoxmbtj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qhfxsbhc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kjkfwvqq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hloueany.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hmsffzlm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3calcbhkd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kaypdsmn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rdxjjlhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tniuytnf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fadhtcle.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hywxchao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tlnkmkjx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vxablpre.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jfvritwc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ckjmfjxh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ioycubyv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3agnjnfmi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3biltcgxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3iccokave.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qclbnwzt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3khmwikis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3scovyewg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xpqzzvyw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hexmqnqo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wsxoteca.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fapiaidp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhmlskiy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3peqxnbrw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iexcnqyp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xxpguayf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cavvyfjd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3duuxkyhu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3blxwbfbk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fjloylim.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qvygfune.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nklojndj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zwffkyrm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ffdeigoy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cuebidjw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrnweneg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awjbramr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bmrjbnqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrlxoaon.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lxjctrvo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fwqqscwd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rmyrpime.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jeillnmk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aipmjxfr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3omkrmogu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ntzvnymg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zdwwmaya.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3futdkjwc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xysfwslk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vmbcjpby.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gnrgupyk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cjemzowk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxvvijtg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhlyjljg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqvkhuv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkgmjyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqsviwu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lnezezad.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frgsfltz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yudfnvxu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3damrmnll.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mnpsuecp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqjlfem.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zmzxdogx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oaqfiamz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mklgcpxl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lexoacdr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vgmxmnvk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgsjbaka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kylhfxtk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfltyfuq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eeppweqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtsofdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ahtqvfwg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vejzhupg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tlietiwz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qhyiysln.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kmxdpgqz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vjvqjcds.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqjwmim.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3itzqpwzv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hkgbionn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ucixqjqb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3efwzbshy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bbyboxzg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csjjfleq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqanpmdl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mvxnmhvd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jflnlbha.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fsbikvvl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nimwwayz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ybvwontv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lwajumfv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qajlvbbv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3awycphbi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xvymvavl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3paoptbyg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cukvtqyc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3revwlywz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fmwifqbe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fzkbsped.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gsqbduhv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mmayuwcg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yulufanq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mazrbnqc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pluqalqn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3yarebrcc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lczozdwj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqtqbgc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kfqxqszz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukkdtkoh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fuyzwtza.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ekeuecqj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcmzfepo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bdfcjriy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bypmadqw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3esnflxzo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wzfcawbb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbktwz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3puauqktp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dqlpkydd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xkihfsqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xnhnhpfn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqbyjee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsbrymn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3yrmworhv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gkgsnaaq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aecwcvfv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ktkuhxnq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ruqzhcge.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yrpramay.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxfjudzz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3madeylko.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ubnnsmmu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aixttydd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtgfotmg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dtwrkwzf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbtwyz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kcyqmywm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3helpknro.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3spjntets.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnmqzur.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbstyse.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3idmigoii.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cryebphw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3chcuxdaw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tsjhylaz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mrcgxxnw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mbbbuxhx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ujzpabff.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnhbpmey.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqwyzfkz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pappznhr.html


<!-- 参考信息 -->