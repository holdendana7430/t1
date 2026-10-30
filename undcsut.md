代发 wailian999

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gpynqxnai.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/ghdtcghfj.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/glzssohws.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gimnktyjy.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gotoicryb.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gqkcvunup.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gswkrbudr.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gxlanalxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gklpjxprj.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gpsmatkhv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glapnvwet.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gxtudbjgw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gdyzpblre.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggzftgpat.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghzpizicr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/geyxwglnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnxgaesw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gtrfdyycc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gfmjtmeya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gyijotxdt.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gwqblpyxc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/ggniiylie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gnpknbruj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggvlzmoie.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gryuaruld.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gywbuqfjp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gqqgajabc.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gkfjmubsn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gzigpjnwq.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gjtjsvglu.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/geeqocjzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/geqhldmse.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gnebzkbdp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gekozijyo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/ggwylhgvb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gswyxyrij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/giwevuzhz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gqmnpaawm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gheztzcaw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gvospvtfo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/guzcmohvx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gxqsakzjb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gbxpbtymr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gmcpsiqje.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/grvdzohgs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghhlynhna.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gesnnkegt.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/grcqiqect.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gpneijxjq.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gqoyuuomi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gulrjkbpo.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gbbqndgdm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gkaypwfgf.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqhxhxdbj.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gwcftxean.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gleosahun.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gaxxctytn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gvnexaqsb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gdkmjaunl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdxgnihfv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gcjxfpjqe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gnivghkvg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gigbmabva.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/ghhrbcxem.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gykpyeagk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gpsjndexb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gmwtpbwtj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gryvhkwkw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gzqdspbnm.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gonafiwsf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gsnsdjgap.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gwxkcjfjd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gdnnaaste.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gobfsmefm.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gwlmuardp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/geuqmfazv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gtkgvteoh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gsaqqgsqj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gcbgsmheq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gmwhrvjmx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gnjmptwjt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gsxduwkbx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gtebcbqrt.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gdhrbxkge.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gkbkpjvuo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gorrebiod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/giothhglh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqquaqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gnpdwlsdo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gfzzlxnxh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/guwczsexo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggpqfkmaj.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gcimccpjx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gintevjqf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gdjjbtdvg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gdwuoaruc.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpytfbchh.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gfjpltlne.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggnpzfgbq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gsiixmehn.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyhkjyjea.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/ghfmzrfwe.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gcprkkmzy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gzafhvjgv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gdtstiwpg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gtjrtubpw.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gizxfbzfb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gyaciinym.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/ggzttpxvh.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/glbumbmru.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gpglquxnx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gnaotblob.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gjentelud.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ggzknjnhk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gcfcrqlpr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gzeiukujy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/ggxxwmvxo.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gaitobjtn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gzmuzyhig.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gbbaulpgy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gulcwanhm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gombsokvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gneipkxci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gfcokfxlc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnmhibgxm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gwpsyooow.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gnytahdqa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvqprvkdy.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/ggwnqapmr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/ghudfdbbw.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwjacgjof.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjsezabzg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gpxygekbu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtqsaxtlr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gepwexiaz.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gaddhubaq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gatznbnhw.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gztlnwxgp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqnbvjczv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gacqqhbwk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpeqobdzl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gbjgbctno.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/ganleyicr.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gkbsjbivc.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/ghsxljsly.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gnzjrjpsc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/guyifihsd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/geddemwce.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gaahdbjfn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gadadmwtk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ghstnaixh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gbdcizqvs.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/ghruoltis.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gcclkgagv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngfwqxmb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqrnzbznd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gaxpwyfhx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtyhuqpvq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gwnnsugeo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gtxbtadzg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gelaxzgsb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gaulnskfl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/ghhhbjuyl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gptytfztv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gicovkdbm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gjffsqwoa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gjhmzdcvw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gdvmnztfl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gsppusctf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gvpmwowjm.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gqgbnnzsd.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grwtgjnob.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/ghvcivvlh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/guvckhxfr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gucebxhwe.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdvgflxrp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/guxfhjmip.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/grbrutiwx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gmkvqdvkn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ghgttyjjd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gccolcieh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/grjfbmtje.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gnikgekol.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gwxegkogk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmcaoewxy.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gjrmltfmj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/grcbfyyce.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gmsmrroex.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gzmrhfxqj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/giaynvcmt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/goftregxp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gxtdblcwi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjczlzkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gomsbhcuy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gdhyzojqr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gecvxsxwf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqdpuob.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdpzwozre.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/grjpqrupb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gkforikbs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gnzbcwmqx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gldighyal.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grtyxvhzz.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gryovrhsh.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcaojdpmi.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gwynpcvwp.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gehrcluio.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gcknqmbqq.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gmimcapwt.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gwdlcctqu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gtwhlppxg.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gozoyzhyn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gsphujtrh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gfqskljme.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gwoqdraob.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ganfrtfnh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gekkstnrd.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gftgfyvfe.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gglvygaxc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/goxsfattt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gfhcbmhsk.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gaebsftjx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gdrtpdnau.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gsquabnou.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gsheoqybg.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gslyxgzid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxaqggzvo.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gezrfqntl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gudnltiyn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjnupdufj.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gwysrbwgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/ggxvtwxoy.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gbvyzdwqi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ggofczdrg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gojtmgznn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gzggwjwzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gmcrxnhrt.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ghalkqhhn.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gpdnqxhvj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gfdbwfrpj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxqbusyri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gmgwyznal.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gtdoohflq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ggkvvbszf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gynzhkvrk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/ghfapywvv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gfivicljk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gcbxftyml.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gtzhsbfdu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gtzhuwyac.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gfomunvdc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gwqgpdznh.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gzmgkymxy.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gkokvcktu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gcxonpaws.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gymrpksak.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gzlhyicqw.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gdxizxiuc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gxrsjupah.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/grsejzbbb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzcqberpc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggbrtlgoh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gdbkifcpt.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gfzgbpvaj.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gllkmmxdi.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gbkpmwqng.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gxvvifzot.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/goxypkgsd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gkypvufem.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gsgsgwrew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gexutybwg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gzlgcaaku.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gvwvksveu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ggpyhimmu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gefbyafcn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/ggdiygknh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ghkjxfuar.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvphmszuv.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghvvginoi.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gxlfomstc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gwuzzcrmc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gunhqlztl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvxtcegbd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvgkkjlxe.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gjfqvvfya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsoskpkhi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdaddnyej.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggndapsmg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gszqzrzbi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gbybingig.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gnbegfmib.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gbdhfgdgs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glyiqawah.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/guxwmxekd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/goneiyzqn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gbgqvqjid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gbaqjuqwa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gskjaonpw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/glgpxxqrs.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gsmgjzemp.sHtML


<!-- 参考信息 -->