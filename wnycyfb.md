代发 wailian999

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gvfsywohc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/geeopzzsh.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ghvgiaqcq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gvrjrlexm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gmxyeginv.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gvxttesdk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gpgzxhmrn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gzmffegod.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gawtfqqqk.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gofbfokvz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/giybmpsvw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gomfjgqho.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpasvmxyo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/grsnetpfc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gdxzxaxpf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gdewyhmrq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gpbkluwuf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzaekrdcq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gxquqhdgi.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/glhesezys.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gubhwrhtw.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvrqvrahk.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gjmnjzusx.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnppurnej.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gftaveeha.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpluhxhrx.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbtkbplnt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gjkeoixvh.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gjqbhjkls.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gulpsqocc.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gzolbtzif.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gswcmqckj.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/ghwutltud.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/garegigal.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gnfhaarzy.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gueyltupm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gactdswss.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gxssnjwkb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcctyyfka.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gmdyawnfs.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gzulfuwfz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdeqpkavb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjmkbeuzn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gmsjvtrps.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwtajkify.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwgxmxu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/grmnvpxad.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gniolbafc.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/guivzikqv.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gbgsndfed.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/ghhhkrugu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpuepuklu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyzkeysql.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/grmabvvby.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gcwaszxxf.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ggizotifa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gsojuesav.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/glntvkcjb.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gdxvyjtwq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gdmsattlt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhcvzplp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gfconkltr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gybfhpypu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/guvaxzvkv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gyimjnjry.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gbistjbhu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/guyeweioq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gklrkypsl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gepumvlas.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejkizvtz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmaksqkvo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/giofvlmfx.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/ggcaxoegv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gkcqlpzjv.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gdahervbr.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/geldtzyig.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/goosscgab.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbvqajyyr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ghftfdlpy.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gpfcwjsjm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gxncltlos.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/ggmwewyze.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gnxoovdje.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gimbusjmc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gnkeuyuer.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/ggrpuyaru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gtsejyavf.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gjcrvafij.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gsgtziday.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/globxjemx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/guiqmdzfe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/galelgbtb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdiwfsqta.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gleuihgyt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gzbxgxtpe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/glgxjvivk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/giwhtkiba.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gouzpalxg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gutqqjgao.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gwonqrqdq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gxshekwpz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gwnpdwzir.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbslnduxs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/grsqaqkla.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gvrgierzu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grzsqxert.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfbboiwjq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gixdxinmq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gsasslyrn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gditipanm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gknnbtqut.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gocxigegv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gzvueftot.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gsegokxqz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gzubmtkuq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gzcfqkvcq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gipbbiuco.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gkkrtazyh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gucsyuqxc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gchzbahgi.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gsrqzlenm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gfjknrllt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gfcgdywgp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gbaspwdzq.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gezfrzfzb.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/guongwlyr.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grcgkfznb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/ghasezujl.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gqpbpstwu.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gnaezixsc.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gvbcqurjh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gzbhapxck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gtxmtwzda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gnkmrmknp.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/geqwxuzal.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gtnimdvea.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/grrmfnlpy.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gbugntxix.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/goastuoxq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gvutwxytx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gzdxkcdmi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjaryqfos.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gkddlguxd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gfttsljnq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gnigxfcmq.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gfdwaooxk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gszlqjyxh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gebqgcrpc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/grieiwhkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gnpdtqhor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/grstdizok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzwwwjkjp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwhtucdwv.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gieqoikwz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gevwwxhrb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/ggvqphdgh.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/garmsvghc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gsxjlkpgm.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjthkhird.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gchgmoala.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gdabwoaqg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gjvmodtcu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gvlfdwfcr.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gwmhpfzjh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/ghizoyrff.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/geefryiul.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gzjryfvaa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gugnpqwoj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/grregrfdj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/golpmhjcu.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gechvnirf.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqtyjfoyf.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gpvinagyw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gnxljhkcv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/glscuwlbn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/ggudrvlbp.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gklrndwbn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gtwcofotr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gbdfzhaep.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gigqqyefd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gycofvimw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gucrsbmuu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gsbtrhepe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtrjqoeum.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/grtjssyou.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcbhykodr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gsiyjxrfj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gmoiuqcwk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ghnxrziiw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gescddkxr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gwgyslapr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gjleapgfo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gqqgymkbf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gywtkhlyy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gysamzpbv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gqzrfhrux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gvecsbsdh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gebqqbbyz.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gtohqtpse.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghjxxtbgj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gtxfuhgjs.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gkybjqkgh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gtvuhoqoo.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gubbftuft.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gznmoyplm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjxkywgsv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/guvbvpaww.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gfexriiaa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gymqcawug.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwcegcujm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/ghymyapuu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gnteledsl.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvdmtbein.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gxosctuto.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gxktqbqao.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/grftjnykz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gawzdrioh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gsxftqwzz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gnuuhisru.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gsgidvidt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/geglrldag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/guwdphbad.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gbkqkyexs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtpmzthlb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/geqdlymza.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gwcqhjjey.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gtqbsyego.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gmqfglzlw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gfxkbifxb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gaqckgapy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdqfzbnop.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwgzjnzoy.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnxyiccng.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gahlhyygs.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggcxwyoxv.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gcbqgezyd.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gqquqamua.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzkzmaxij.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gmijyghzi.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gajxfetpr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/guomkeffh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gsiqtkzun.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gijzfaefr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gqhxopiim.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gwlvkmyli.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdongnnvd.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gneyamxco.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gdpxugwdl.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gigmecxsm.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gvpdopmyo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwfjayknz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gtzaplzuw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gafrzpvxw.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gqqcvlzum.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gbaiksilt.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gwgzxytyq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gwqgdykwn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzinclkgk.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gvtfopegi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gydqwwqwc.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gsljcrhuc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/ghpzwulyh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gluohpvxe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gfkpwtiii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gxksqaapp.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gswxppbld.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gwsvpmvrh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gaadsugsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gpdywmzys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/glwcfwsno.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gcagqzytq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gvlzfslem.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gzakxuepf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gydpswiop.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gftfthfbq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gizuexyuh.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/giousrmcm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gypnynsja.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/godxjookl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gvjqrjyjo.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/ghkalzynh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gxbnkcatu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqrsfakw.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gnmfzkzyy.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gfugmdjht.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gmhcrrkra.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gtzskfwmx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gzkbiixfx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gscmktwdf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/grqvzxuxq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ghipzitps.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gongeydmz.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gvflnoyaz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gbzybhczs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gqgrnmfan.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gapfjhlbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gmakomiug.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gnfohilii.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gpeeilclu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gbizglrhi.sHtML


<!-- 参考信息 -->