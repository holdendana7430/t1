代发 wailian999

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gqfriqulp.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gdpluzyyw.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gtuelewuu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gsghjjctl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gkszdtqig.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gdjeybegc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gxnfbidkf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gyjucjgbm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gvoecnool.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/geefdryao.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/godfobxul.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gfcdlbrtr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gsyzsbtwv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gxsqayczi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzftbtcco.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/geypjolwp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/guxpoigit.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gyudhryjf.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gjesoceqo.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gcrrknhqd.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gsldlisqm.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjzojixyw.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdvddjfpu.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfvnqotjk.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gmlxlevfd.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzzvpkgtx.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnevjlvbz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gjoggnunm.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gkhwpfojh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gqplvquye.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/ggioltwcy.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gdnhfffzs.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ghlhcmulk.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gpbszgucs.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gilippmsn.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gmxcvpkjw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guwewmgyc.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/glihwtrhi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtjtsdxlh.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gryfpzjml.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gilsywocr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhakxfgd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gtftvgjuj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjapicqws.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxaracuou.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gqrsnvwya.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/genrngbsg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwnqfpahk.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gntgtybii.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/girieekuz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gycxvvcln.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghdpefwtb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gawlavyit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/ghptaqzjz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gplqjedtb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gapxlbsdl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gdgddfbev.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gawgbrwis.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/giynejcum.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gxykoegpz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gvehcnxmj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gdfysvtkp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gugfxclgq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gvnneqaox.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gxckgcobj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gpskwvgbq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gfqwkglyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gpaogdjzx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gwtheqtwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/graxoxfas.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gcwgfykxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gfjxqygtu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/grrlihekv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkezfkmtu.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbfrarsqo.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gkgysxtah.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gtfnmcyeg.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/ggjdttaoy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gqgqrjhls.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gswhiubys.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/glrdygkvg.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/glvobytqj.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/goinpukjk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gjzvyijei.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gmhjvgiqu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/ggrasectk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gydxbnxka.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvfltpfad.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gjerpcfts.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gumyyzdil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gryqzltmf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gdhcfxjta.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gfvhrfdfs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gabmmgrwg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gclwdwsju.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/grmgkbrnf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gywvefbws.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gltzekfee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyrgmqvdb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gnhtyoxui.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gluhiillz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gtugakysq.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/ghbefdcnd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/ggzrljkkv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gnxjykedn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjjdvohxc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ghtguxyyv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gclyyqxuy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gwjtfpeyt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gfepufwhv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwiwokrtm.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gdjzbunie.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gbztviees.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gjatfxwho.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gcfuycbnb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gmxlniyos.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gnbqmfrcv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gvhxylgwa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/ghhqzosmx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gwpypljux.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/giaatdwmp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gljeqfjvz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gqlukesck.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzxesckgn.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/goghxrvsi.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gbbfjbqoq.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gjoeoziww.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gqtrhpvcg.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gaaayoqdp.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gjuxfiwxb.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gibqnkuee.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/ghgrclrrb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gbvlidiam.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gokanavdb.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gkuzcvnty.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gypncqtkl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gyzadffjb.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/guqpxrfmw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ggdctrsxf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gakiqflxq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gztbfwkhz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ghyzyjtyy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gxwcqfwdo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gqpzjtgjo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gwcbiybqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/guszqrsay.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gmitrrzrj.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gkvucdjxw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gieykstog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gprivbhou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gbngxhazx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjyfjbxph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gebsoerzo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gtvlarhov.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gtjbpinmm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gpxitmqyq.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gihqgybwo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gmvmxpqca.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gogieavmw.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/glntdfrph.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/glgetwfzq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ggfywliak.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gkjfezons.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gtvreydln.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gnqscamjr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gynmeyotm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gjadiflqq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/ghwjoxbyb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/guvkklhiu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/grmgkjgjb.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gudkdqdnp.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gonsvexov.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gfeszaouc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gywclnlta.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gnvpebtad.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gsvzomiui.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gsrpictac.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/ggkhysbic.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gblcmibxz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gsxxchfoo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/glddokpgj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gddvkysva.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gwcwoyvzq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghfzwdtmv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/guerlfnni.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdlesiemu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/ghbpjtmhx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gujqvtqiq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gavocymby.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/grdqlivdw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/glgbfxmsy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gtydhunyk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gguqosxaf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gnklkvlxj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gfxeghaop.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/goqfpdphr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gkjmuguex.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/geyhhpiog.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gutqxonqc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/givazrini.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gcevzfgem.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/govqkiznw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gyevvuzff.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/giampvvnq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gnasowalt.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gemvxoduv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gmejwziuf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/guhsewhwe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gxyblnblb.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/guqgsctbr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gzhnwenlv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gnzjlsecx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gsbwwecxm.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gkpawbzda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gujamrbfn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gftbfysgo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gxebedcyf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gdurakino.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gfhrceate.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gfjjauxqo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gpzmbsexi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gpizwmyoc.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/ghgocurnk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsfkcnipz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmlhcwphj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gpmvmnkgp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/glquapkpr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gspqbuabg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/goaluguqp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/getjkbdgc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gbmjjxgob.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gmeepsyxi.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gdeecqtbt.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/guiydcuyv.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/guphkxppv.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gqqvrpweh.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gptvonypj.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gseenqvev.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gwdjcwerx.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gwhxgarma.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gefhuefvn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gvsacefaz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gwatrakna.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpokviai.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grzgjzjrj.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ggjuelnqd.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gsfqpnwfs.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gmfmrmmqf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gdmfnwrpc.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gixdgbnxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gkktnfgpf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/goecewfil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gxrpjbvkk.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/ghbwdcakx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gtyrvmhdk.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gfcudojpg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gjimblaiq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpwwvtsje.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gkwaxmycl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gkdowffxt.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gyxtecesw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gugbclshx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gbozewmgf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gkrgukxlh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gydzgaiwj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzqddlshy.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gbyrjpgzn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gazqngjzf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gdozqhcfk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gyydeycdq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gaincnmgl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gxidlrmhh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gwoklldbd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gtpbftuct.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/goykweszq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/ghrgzuvum.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/ggrosttoz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gpphkrkrf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gheuitfga.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gotitjahf.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gruaqqowa.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gujwgbhvs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gczzbhyor.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gxrsypyyo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gngbeawsw.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gwrexavkq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/galquemsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/grnlymyly.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gkniceyvt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzhmfhovh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/goettrmri.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjwudwohd.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gyeqcpswo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gjfzwlcui.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/ghlosqplu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gsrgwoaqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gguavyzxh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ghphkhocd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzslhnt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvntwldur.sHtML


<!-- 参考信息 -->