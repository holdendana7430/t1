代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/gisereuxq.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gdjductbu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfbgkvyyl.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/glavnqvvh.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gzckapzqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmfpegvkt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gflcvmtji.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmtiytvbo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmnzutxls.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gyumnkfkv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gimojcggb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjwrpezru.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/ggntgnjfd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/goxjayxab.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gxdxgsgue.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gzfmdodgm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gclhxmsdj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gzvwehnkf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gieeybjeq.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ggqnhdvjf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/govgzizee.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/glukelxhx.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gwllfnekh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gyvjodbxo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gwanexnum.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbfmbvjnz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gobcaknql.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gnzadbcbp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gimefwdzi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gutytaqpy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gtzswbxla.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gcuxuoyns.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gkleinptq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/guqynugab.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gryrvztve.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gwragxies.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gocwtdiaa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjhpriomy.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdfhdmarz.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gixwrhwuu.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gjgaxjbho.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gxjnpnoab.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gsuwhukpe.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gikovlfum.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gklxhxati.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gtlggjmrw.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/guwibaegk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gtflyomki.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gypgyyuwe.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gpvzpkzxd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/ghamypeqi.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/goukgqdpe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gjyxymoez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gugyyveuq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gdedmnyar.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gqaeiykhh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/goefraehc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/grxurgmld.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gvrmzhyyw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/goqjsdukr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrizfbi.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gtugojvoc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gwnlzsfoq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gebicsykk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gejacxbvy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/grmypkmkr.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gvjqgoyuy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gcltukhlw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gosgygtiy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gyrxbfxad.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gkvgfxhkl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gddrpgfxv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gwpbfxcsb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gbnwxslhg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gdbhfnyos.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmjnakx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/glittixjd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gjyzkmtxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gfakrxbbb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gcbwzdrsb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/ghvmeaxzg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/glrlwdbka.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gvjdmtbms.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gypurlgyg.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gwqvcrtdu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gtlwdaers.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gdoazpwqf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/grxcffstw.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gyftktdpd.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gcwkwgjta.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtyeqjswl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gkxovtrrq.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpyurhivh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gkvkuigpu.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gkvynpevq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/grsxtpygs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gzptxqcuf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gzrwpsqfy.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/goarorxum.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/ggatvcfqw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gfsrhspzi.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gmkbxtavx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gqzhsgrbu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gdmueqqei.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gtrqoicwq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gkrsbfear.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsdobwz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/grprzknwt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gdumfvbfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/giibebojd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxucxgnme.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gevdwnbzu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gvkskusib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gshplxvew.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/ggegziimm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcyqkgmin.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtzqjnvuy.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gojfhlcgp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gqneptvqt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gezxagloq.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/goavqkdoh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gbhsgorvd.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gnozbedih.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfycdpfqc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gnuluvoew.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gghwrhwwa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gtrwrfwpl.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gqmuwaswg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gufrebzit.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gueatnsoi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gvnyrbbjv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gmkragsum.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gnvtkwdyh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gwkjgrabt.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gcvxngbuj.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gfwzrmfgr.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gcikfxcsp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gyjwdhbut.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gjhwomwtz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gbtmraqac.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gnhmmpfcj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gdqwdvpvs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/glladfxer.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gnpkwowfn.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gsdzqnuoz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gytfukjbd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyadhstcm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaicmozcx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gfwvztzkc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsecnkiry.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/glgsqnhsi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gwbjwyrmt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/girbboxfc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gwtfafhyy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gjztytuuf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gkcsnrivf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gfqtsyfcl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gdnadbxwv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gexerkbwb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/ggezhuouz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gisjsazap.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gvnuknpwn.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gpazfkyqu.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gwckixqys.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gsftelclo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gynytqagl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gftgflpha.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gfriejpoy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/govrouags.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxusewhjv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/glsptllaq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gxgyuymns.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdacddtiw.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfolstdip.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gsmdhnesp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gccdrdqxn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghlfhhkro.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjynkmfox.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gqdzojkfh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gwrezbgeo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gilijpzly.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gcrebffut.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjdoujiwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/glfwsfjck.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/glwnjgoos.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gdthphitr.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gqfsfceux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gvhwhcsit.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gcjixswjv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvqhqelje.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gbzxfyool.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpoqgdae.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gimlctzrz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gsrgvxpuy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmguiaple.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/goyzpmyxn.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gphnnuxkj.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gizndzvff.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdvllvjrh.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gebnzgxrh.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gtjerjmml.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gycyvylmo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdmvzrkqb.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gqybicgft.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gbtnihrbz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gzxikkrqc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gojueczua.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxuusdvde.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbryvwkla.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ggxugdznw.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/ghayjkoha.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gmltizeve.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfuqsdysb.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gjlplmpgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gocmhnhmi.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/glhezktsi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gweysxaqv.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gtrlhqgci.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/ggabbqkja.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/goigkpplv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gqdfzxyga.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyoelgexv.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/guqulurlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/grxdtpzxj.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/garefeopv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gkxsbhiil.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gdzcrqtlq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gbiizjgil.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gwbyddayn.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gtntquiyy.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/guxufjblx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gkzwbnibd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gssegrlgj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gcgqnvvsk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gltvoedpy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmsboojsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gzbibkbbf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gacpuaetc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gupzgxrec.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gtzkxsnrm.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gzpzsdcnj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gqgovjjbz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghdixuhom.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gmplzpyad.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gfuqkbtpa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gmzbtraof.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gaptrpuof.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmylszejs.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghdhoijgv.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gjnrgtupa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gbqxhucxn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gjtqxecei.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvmcoxpiy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gsvhwafjs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gjeufggci.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/glinzmywp.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gibbrubnz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gllhxjnbg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gbnqdushp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvqvvprvy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gwhfiugxs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gkhasaxew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/grapaigzs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/ggjggkonw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gxedbxavq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/ghxzwflqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/glslmlykc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gyouimfmx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gylkridlv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gzdwhsifp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/goxxhrkgn.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gemnmhxdu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gidilsboj.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gyomykfmh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gtbsjblgv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/guiexngxh.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gsztlrzvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gllkubpkd.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gkunxoyne.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbzprfpol.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gfgbcwzuh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gdwrifton.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gevoouieb.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gwbtuqmpw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gaalrbcar.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gmcynvmkc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/glycdulqe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gncvwqutc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gnetawfqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gffuesbfh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/ggfhtfpvj.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/guhjhondw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/guekhxlot.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gisuxbokw.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gwvgzckrs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gjrdvlpmp.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gxcfbxxit.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gqnsonoxj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbxktonyi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/grgoecsnx.sHtML


<!-- 参考信息 -->