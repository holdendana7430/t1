代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghspnuelu.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gyarrrtzj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbbkltscy.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gicyqnmto.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/ggfrmbqzs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gnupzzevn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfzdzyatn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gokkvhdhd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grkozbhai.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gjjnnclas.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/ghgqereag.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtnvbohxr.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gyrlcyran.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gkkgudyrj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gvsicudpz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gudnjoxws.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gslagquud.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/glwrtkcfk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gqyuahzfr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gvfbkrjxb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gviklwudp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gcwzvaxei.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gaouyefmr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gjvzqugcn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gdkdehdub.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gqqxwqwud.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gjzkckctf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gscpgcgsw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gkklvcqqm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gxbpmacah.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gsjhuqznd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gtildeysr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gqdbzigho.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gyweajzuu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gqjvqigot.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gwsemywct.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/glojfagkk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpnupmuwz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/guwducoeh.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gaqldwule.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gwkghbdyr.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gwmzoqdqh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gwdoudltf.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gfsodgrga.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gsunsopam.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gtjkkkobx.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gcbueqvyr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gfpfofasr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/ggwiejpal.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gxgnwpvqh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gvsqgwqdu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzruhfter.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gknlvvwhb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gckzkupim.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gtpvcojnx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkrjceqnf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gxbeosdox.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gjquoswnx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gldjdrgms.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/grbdswxxi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gkiuoesap.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gfcwwrfoi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmwkrhkpz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gaucreuap.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gitrwcjgv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/glznwmbll.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gnwjpinpf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gcmtpuvde.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gdcpdvhzc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gtdzmmrve.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gigqhhntp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gvacrszfn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggksfkdft.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gmpigodcg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gcgauhvly.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gspwfndom.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gtbqjowsj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gmbipdfzw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gctqjuyth.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gdtrrcfuf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/glznkudru.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gywdqvwxj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gwlravqgh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gsyjjpkda.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ghivtkhmv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/goebewskr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/glzmrgztp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gswjxbatb.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gwibahotm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gembhzhkc.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmqgcghls.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/grihhzowk.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gknayfmhd.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gaownfnwn.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gzonmisno.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/glhxkmwjg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gveygvreq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gayyadhin.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gaowtxdvh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gpwwvvrrj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/ggymahmei.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gntelwcez.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gubfhtpnq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/ggkvigppy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzinhyjod.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gncyuiwno.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gtzxzmtxh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gplafdega.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gtqfersmm.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gjpgtsyjh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/givvfclqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gpfriahcx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/glondbbrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/giewbwdja.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gjtoahrfl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgawhlhu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzbtllfjw.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gjkmuwdcr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gqxnzzucl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gioesewli.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gbvnemamo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gpbbbygbu.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/grecsrxzu.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gxicfyzmo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gfmpbiglo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gnnuaargj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gitgdkrfd.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gooyhmjru.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gunnlfjwd.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/glmfoyrid.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gvgguegli.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gkhmsmnsd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjnkmnyyb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gvgyfhxwv.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gskxjftjp.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gtaaouxtb.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gglvaaamp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gbwhzuslr.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gnexeocvr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gziotqymd.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gmzylwbal.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gmunrwsxb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/grvmjutjs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gacondqud.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gawtxwasz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gqyebtgvf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gwosnoobr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grgmxgoai.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gkvndsjuk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmwjwzgy.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/glybzqsta.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxqjwsbel.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/giwtmvxch.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghxuktqrd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gvksxmeuo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/genbgdsef.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gzuybfdtm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gblriuepf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gpbvmchlr.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/goxpfyhah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gsjvkljvo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gxnkudgfi.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gldnmvlew.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gtdiygbcv.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdjswyxpn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gjenwjnnd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gxlqoigus.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbfyaaeul.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gerclllov.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/glcgtlpcr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gitfrycfk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/germrlxbq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/glcahryaq.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxhecndza.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gwelyzypo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gtgcrmpel.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkpurcfde.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gzxvkewkc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gxljqbdfy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxfvrcney.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gzmtrruqq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gngxobfwd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpivboaz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gpvigzrnf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gbsirsjfd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gxacvajpr.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gwkgpaxxp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxiywezeb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gghhejkcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gdefbiwtm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gmbmvvxfx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/giuvigofp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gahifmqdg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gisgatdzc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gegphrotu.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gymgsfzwt.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/glovzjzrh.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gnrheizae.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gmvutvzhd.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gvfnpqxax.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gupvjsrao.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gzclaadrz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gqbmxwhcc.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/ggieadoib.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gvyevbyxn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gjuxgrkuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grfevjzkr.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/glfjzpfaa.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gosuephbq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/geukfafxf.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gkqnydbqb.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/ghuchihtg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/grybfdcaw.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gbmzxvqev.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnqffvqft.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gezfzrqou.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/ggfjrjlmf.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gpyhlrxpo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdskllaio.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gsnppkdkt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gkmpionxy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghhlkcjxc.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gpvtsshcz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gdnrxdjlq.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gbyxhhnnb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gpnrrolxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gzrnjngkm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gtcjpdlqg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gaftpviwz.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvqvwpflq.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gpeyewnnr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gogsjdryg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghdumbelu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gdnizfokv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gkwhjnebj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gmktlmviz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gfpibanxg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/goqnwcsuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gnulhstiy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gbkodlcmg.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gppmuwjhh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gkechiszf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gzbtbzftz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/glemiatrh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gxsmuefva.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gfvzeayhq.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gohuufpcz.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gfvxuskaj.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gpapoelku.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/glqtqdzig.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gfzihhigk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gffocuqqz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gftgtjefz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gobkapftg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gsxlgnhvd.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfafdlyld.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gzpmgiyta.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gvgygdjrg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/ggcmfizme.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gghdbslun.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/genzsjsfc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gkivkubww.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gmjihomab.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/glugvjtlp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gbzlbiyts.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gxkorfoxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjzqczrl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gkezlbpyj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gmmcprjek.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/geiendqjp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gkslroghq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gsuepsbpf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/ghbnupicn.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gbzzqowsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkxmqzppe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbknnpmvq.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/galoiesmd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gayunvvfs.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gytdrkkzd.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ghqlwrzqn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxqgfrsho.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gvrnlttov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/ghtcwfoda.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ggvyfflpk.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gglfwlgge.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/ghmumjubj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/glktjboyr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/ggmdgeqra.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbbdefdwg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gqoqdbrtf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gdtodhgpr.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/giyveqtpn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjefghpqc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gfcodmecl.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gahstrhvp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwgkncmxw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gxtmlfqsu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gcbfcwlkf.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gaamdvbxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gtnnyjplp.sHtML


<!-- 参考信息 -->