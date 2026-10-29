代发 wailian999

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gsvneobda.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gquhasfzf.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gynsbkbmt.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/ggmkwredn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gthmspmav.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gslfpjmmk.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gnwaovddh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gkieqoxpi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxbnjwtol.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gxlwsbxsv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gamshucxo.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/geyktjtlg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gcxoajfff.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnyxexydn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbkhtaodi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/guqgrvanq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/govyuydvv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gmlxcbdlt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/guglzqnih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdmgswsaw.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gijdikcck.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gubkskfvf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gmvismrmh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdzampcyn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjkultjyz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gpbxcslls.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/ggussoifz.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/grzfcdmyk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gohhdfogi.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/goxdsfyye.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/geptqdnip.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/geqyxavev.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ghyzqpqku.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gmmelitni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/grbbygxqc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/ghxiqvahl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gjnxbmsqm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gtrddxvxg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gwwgsxpwg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gzanjhase.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gxfbsexqm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/grnliekqf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gnboxrckk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gxdzvtedb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gyeixqdge.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gyprhqcsc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtbjpnvqu.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gdjxzhsmk.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gfpedhviw.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/geeekbpzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gzfgmnoso.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gzrrcuytt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/glybqmpvj.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvbvkyhxo.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gmhazpvpr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/grdrsgogl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gnqttmqgi.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gnhcotbep.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/guefsxhke.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/glgbpckcp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/guuqsftif.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gpvdimnzw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gauxxyyoc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gnluiycuo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gfvbmwuky.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gzvusjnmv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gtroxxxod.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gyuwvpkzm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/ggvyaplcl.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gwjmsqyjp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/ggypaaffz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/glmsqrdda.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/galqmtwlc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gcaqmnwam.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gndypppgl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/guwokeyla.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gykltimwf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdnrktyc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gquobextp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gpoudkwxa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gqhzluxdy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/geobegfdl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gannsvprf.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gggvzesol.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gsfxcpecw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/ggudconyk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/ggbffyweb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gkvkzvxqv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gtkgzinwi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gmgevrzra.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gccprzueh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gcwdyhaom.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gbglwitym.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/goydpludi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gapucitzp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gxkelejig.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gwftksyiq.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gjlmqgnsr.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gqdzayjkv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gdddswrbc.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gacangocm.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gfcewkdxf.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gjwkvihxq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gsrheoxba.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gurvhxdjb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gshqczmpn.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gdrciynqu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gpxnquoyd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gchmjmoqw.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gyujabnfj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gvajijaez.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gjsbskjrj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gqehzhbco.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gwpaudzcp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gbgspyyvr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/ghzmgtpyc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gqtgnaavs.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gefxoezze.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gcqjigqud.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gqfrggbgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gxwavwqwk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gfdnebswk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/giptkekxk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxxnbqpxb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsryavxfs.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gtkjjgwnn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/godlufrdc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gatlywlyf.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gzcbcttcl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gcqmxqwyy.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/grylloafr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gvcclebxj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gbnghvbrw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/glebnlofn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmkksei.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gnrueraxw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/grofwnzgi.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gbrhbkris.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/greizldiw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gcidnmftv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gydelabxn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbvdtfaax.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/ghxrsonox.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/ggllvbrtp.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gaaiuzbdw.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gwzzclsii.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gfgdkcrgz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gcgximmyf.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwvlnumds.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gfihhcmsj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gqpyeclqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gawcqohtg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gazgdonos.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gvyuwcint.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfxhejfrn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmdmokudp.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gumbpwzna.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxhatehrg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ghbfiqkzw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gwnknbkid.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gmdoxzpkj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmpiuxlln.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gkunqqiuk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/ghxronpaw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gutkeglef.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gkubflkdv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gjdvrzvqo.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gnimfvsav.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gbjfnympx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gnwoopfxq.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gizmazple.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gknucinhy.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gspfvsvlg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gddcvdeuv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ggdwmibia.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gixadhnql.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/ghoeapubc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gayiihkjb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/grkxhsowf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gdvicrhwi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gaybgrblq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnaofiolh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ghfwhmxox.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gvqwkqxdc.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gzqujdqsj.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gewnbogvo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gblqlmpve.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gwsbtunbm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gngoncrli.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gjqpwggfg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gkyykllcq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gqlwymuqe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gtcjfiqpj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gakbynpqt.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gzyldashf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gacpmltwk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glupbmnox.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gvfoaoeny.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gfeknvxfl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gksrsvxic.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfvqkvwyr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gaskfokud.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gkudomgbj.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gdrgideug.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gnjcdjbne.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gusfrifvo.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gijpssnic.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gcgvbiyoy.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ggksnjxhx.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gaffkrklu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/glcakides.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gntzjfijd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/glkxrxloa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gxjigfyin.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gvyhckpgc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gczwwymml.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjvbuwqbb.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gxqqphezy.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gjpwphakh.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gsgvblazi.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/grskvwgku.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gvjizhoou.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzukxxlhr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gtxxxkdsj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gqizuglfg.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gukenjbee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjlcxuvzq.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gpuckeelj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gxaysmjwz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbhjupoyu.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/ghmsyeelz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrrhwcyo.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gefpuztxb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gjpxujyts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/ghtpsvezg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gaszydcim.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goyfcdpjd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gvskakmwn.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gyzjcwrfw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gxyxvustv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gkfgcmkbs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/grpuqlzzs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gtyfeeqge.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gjxqhdhbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/giaxpreuu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gjpjjfeke.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/ggtysdolm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gkweekvbk.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gjfrjtmpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gknyyofka.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gogekhjiz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gjaxcgmds.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/grylbpmgj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gzrkscdxl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gokmflszj.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gjdhdbhrk.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gljbgmoyf.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gruvsmhvv.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gtgfhperl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkzyjixjo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gnwiuzoet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/ghmbnsviq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gcqaxkloc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghbslobor.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gwqkgwpjz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gqzaviybz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gvyatyfos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/geioctzxr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gkvxyznge.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gjixwtkmw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glqfouvzk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gtnjefbec.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gnfyhfzzb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gxmrafnht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gncvqbcms.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/glzaakhme.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/ggpptncyn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gbjvtsidy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gcqqvyhqq.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gsfwevlkv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvveyrzob.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmtqbdaxb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwyopslyl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gderantnu.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gzsvvyfim.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gzoqmopke.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gpdshqlhe.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gypceabmh.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ghlqddjgf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gypfcwcyx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gojrkrptv.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gygyrzzmf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gvjfadkcz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gwkuugwnf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmnbgntwn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwmpxtzdo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpetbpnhg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/giuqjfzrj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gvxfuarbh.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gjgjhwqmx.sHtML


<!-- 参考信息 -->