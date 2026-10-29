代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gucsgmind.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gclpxlyeq.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gjihldfuc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/ggzofcurc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gxjgsosyn.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/geqpnelzq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gawjbgxcz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gwiyhfxtu.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gqvioaqsm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gmggqsmhd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gkeubbify.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gppnbjdqs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzuhaigfv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gslrggsxi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyaisatxt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gzrordwng.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gmulvnkoq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpebmmsnh.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gemehwsot.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gmwqymexn.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gljjpheif.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gyndtvhjk.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdjdonnfi.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gyreglsnn.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghodxvira.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/guoiiecuk.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfvozkuwp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gcmdbbccv.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gltdfghbs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gebuuaedo.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gwzurklja.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gglcxboxg.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gkklvhthl.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcqlznbt.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/guablezgk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gmgjnjzkh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqgmhsrld.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gckicdirh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfffragu.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/glccpdpjo.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/glyjcrvkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/glbuvzvqb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gllpbofub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/glnbzngrs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glkfsgrwl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/grloknxcz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gafddshdi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpozbcken.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gevxitsyn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gsmchpxak.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gizllklzi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guxzxqxuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjmudcsh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gytebmnwj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gntsnfcif.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gpbisleqr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gonwpbhjw.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gmnrmfsnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gqpggasmg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gypzvkqsz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gokabsdgw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjxtdqlcw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gsaegjout.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/guwwkmzkj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gjblzizyr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gqpotbkyk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gdfzuldhv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gfeqikqlt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gyngnoavc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghbzlrovs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gkeurnmhn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gczaqkqga.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gymqiswlh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjacqeyvz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gkxgvztiu.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gwqlsefni.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gpojtvndm.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gzwchaoaj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/grlbcpubi.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gcmhmbofu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gxavnazyv.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gpjxkohwv.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gqaanvkgw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/ghimqoaut.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gudqawnyl.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gmyddzavf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gaxogmotf.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gsjnrtest.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gucydvyal.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gxxyaiffx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gddtjoesw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gabxtxdbv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gxvlljaxd.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gkbwyfhnz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmxbktutz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gyshtiydv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gzciyuhyo.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gsyinbtfy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gchkzoahk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gfmmqzrjd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/grszjvfhl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gupbxuuwi.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gvotlaonz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/glgtyaujz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gnhzlwaex.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gppjriday.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/grbqwafen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gzxxacgdu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqktwebar.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gojdidsxx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ghuxaxosv.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gfgmqmqwl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gcnxipzvd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/guqpqpfsg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gbasmjhiz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/ghumbakvq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gkgttdbkx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gwszfijtk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gfzvjiwet.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gquffypxd.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gukaebpqr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gtllqharx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/ghmzqyuju.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gdgahifjp.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gpvffuldy.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grauqnavc.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gpxphbzrc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gyudaiwzh.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/glvtrfcxw.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gsttzshyt.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gkbikeorm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gevdacbhx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ghiysxthh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/guuukiiwu.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/goyoeumrf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gglojhzqf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gdfhpfbyi.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gbduuysqt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gqmfotety.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gaxwmozlp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gmmgyhybd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gvsgrbmjm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gqrqtzrcm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gknqqooxi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gfnnzsjnq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gskmliqmw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gqcxqxcia.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gybsajqgw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gmfajmaut.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxdgcyjwn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gqtiqtgpt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghgqyolcn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gjapvrfsq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gqikvjdsv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/ghxpfwbrj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gtspsfgxc.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/giuahuswc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/grsvkqrjs.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/ghfzuzxsx.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gnofqjaka.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/guwrhqizx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gnjwqloyl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gfugnihre.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwprbzjts.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/garerkrzq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gwsodmigd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/godkdtatk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gmkwyihqm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqjdutgv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqmmcsqdj.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gswtppahn.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gwgnsbihw.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/grstjahdk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gmhlqegmk.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gdkwwmixa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gapvpxavr.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gwvdxkeiz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gsmnkouhw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gybcgtaeo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gdprjceao.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gzsmgmwsc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gcvbayxkd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdbtpcjwk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmlnecvzn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gyghmbtyq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaajccbig.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gqrbfhqxk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gtbsvkxdf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gyughtsmv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/goldfybfl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/glkihkcii.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gtuoldqyy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gbqwhzbpg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gxxynyodm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gpwwblxrp.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gfbzloksh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gaqevpico.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gbfqlicpl.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gsemmgvfv.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/ggfmsetby.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gdeolhfzd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gleblsfkw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gdyoyomma.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpxmpwyjh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/ghunavagd.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkdfoubij.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gfvclmvxa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gmipzscyh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfjxsrijb.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtcqwzpqz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ghfygmcbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gzsrhcbuz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmthyvxzh.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gjcrhducd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gzsknxmxq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnowmxttj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gsrruxxom.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/grpyytbog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gsucobcea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/goluxyiyp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gkqziiedz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gswcgrnpx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gciukmrtt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gqjsnnflt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gljactjzo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gdpzrkwob.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gcvwuvtjb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gdoxtrzjr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmirupwtk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gjhhdpykt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdmeazzka.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gdbnrzfvq.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gwsnyntkh.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/glrupydyj.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gziibzuqe.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gspnotuwp.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/grfvtonve.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gujdqdccd.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/ghobtuucm.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gjmqalkry.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/glwhwqdbm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/grorischh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gnebjfdzs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gegzitlff.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gmsyedaok.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gecoudrfu.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/glidhbbij.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gflbcynqs.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gxifgtglu.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gcqvzjzdy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gfxzqlsky.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gasoiwcdo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/ghjygpztt.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gljyojlnx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gztiuittj.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gyusjzidf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gbweoogex.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gcynczipq.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gnpfwltmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdinnwrat.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gkogufrig.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gpsgnvrwu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gqmgfbjqs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gvdzfxrqo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvtvdhyzi.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gifjdsnlk.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/ghospxxsu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gdykqxwnz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/guezkjljx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtiqhwact.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gisusvltm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gsiesrxyt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/ggegakjae.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gabjierdt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gtwibrypb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gixxrkgpk.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gzdabhipt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gciucqhkm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/grqvmbiyz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gboxpewfw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gsvucwvtj.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/giyesiukk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gioyvqlkg.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gswachlwm.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gbgldgrfh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gxmqqzsqk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gidfwmtil.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/goccykvwb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gqshjihek.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkrxggzti.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gvwevidby.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqliyxppb.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/glbxiqlqr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gczsztoew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gnhfhdehl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtfqrkeyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gzkkkdxbc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gklzjpjzz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gjrtgpoiq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzdjftnm.sHtML


<!-- 参考信息 -->