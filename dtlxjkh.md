代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gcasszgvk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gmyompljj.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/grctlltmj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/giuoxetec.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gfjqdspzf.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gihzxtaop.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gnixxfoal.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gkpwvxvdm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gbcpexzap.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gtrdmytgr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gonttihjl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gdeqkamfv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gfnzkaabg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvjclttdn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gvlotegfr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gbednwrpy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gcuxcgorx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gcpvemynd.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gqqqwyaee.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gbbmtcmnw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gfeczdnbt.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghmreyits.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gfnxuiyqi.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjfuwdgvn.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ggdrvnaon.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtnxnmtqb.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/guhlzymcq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gxwokarke.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gtblvazbh.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/glfnpcrvf.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gjqvcbxzg.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/ggwqsxgtf.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gxpoxofys.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gflhxetxk.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gvcgxzfcx.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gzjzdokwl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gixsqdaxo.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkfllxl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmnqvocjn.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/goxanvpho.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gskssmqrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/garduwhso.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtwpubszz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvykoverw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggoirpvjh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/goonuuwmi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gavsdwqwq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghpcrwglg.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/ghfjenrrg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gjdnjacfn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/ghwlocgmm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gaofpuguc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gielmnjqx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/giblaxyzr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gdkleraxa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/glsbxqdwj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/ganmtsuiy.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gxmwcikrn.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gkpqjnltl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gdobzdcpw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gvmasepxj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gtclacupf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gndreytcl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gmxifnhbl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gjxdnvfyv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gjmzcksrj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gyvrqlyeq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gznikosqu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gvdckynrx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gkazhglbz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gltfvclnb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gwzqsjptf.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gcfhhjodt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gwxopvbbz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqduxkarp.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gzycpesgi.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gvhymlnng.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/ggjcxtjux.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gpompgdac.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gxsmeckyo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/glqwsaxow.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gyuwmndod.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gcbnnabpj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gffqkgtic.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gmazygsay.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/ggtnbwrsk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gjbgzwjqw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwldytlcm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gppewklsw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gyjmqyykw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gwitpasta.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gclizrraq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/griinoadl.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/grmazfytg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gikjcvspe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gierszzmu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gavtbtbsh.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gruczkvkc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkvuojnvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/guhhrbqey.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gouxsesci.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/ggmyffnkv.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gqtxpbddk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gzykwkudg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gvuulanid.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gepmtjygi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gaunsdxzc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gnivmraay.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gntxnpnaj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvmbqbhew.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gsthhlyhr.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gzyhxrezo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gekuqpugd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gnghkekag.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/ghlvsdzzq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gtlzbdiuv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gchrodmvv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gsumdoglc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbyquqwsq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/groaqzhxq.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/golrnacbt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gnhirxvag.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/ggyjnvqpx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gthprspfg.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gcbrlgzjf.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gkjcufsoa.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gpuqvhskd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gkqnvmtfk.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gergcdfxq.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/geakrmdun.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gvrbfqyhq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/guwyrwnpk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gglhlxcfl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gjihttqmd.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gtdrogncy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/guqboxljn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gbnehucce.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gvdisnkak.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gjarbdaib.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/guprebotp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gditpeeqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gvozbmblk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gxupsxnjr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gmtnadnhr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gzwqcbkxz.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gpcxmzkjc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gvjltzufj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/ghyqmcoae.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gqfthxgth.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gvkfmypek.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gjpjdyzoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkowsjatt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkuilzzkn.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gujmeebog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/geybbiicu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gfctuxdir.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/goddxqvot.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/ghimgtpgn.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gwdsxlsds.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gqpvnnhsi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gozgnoqoh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gfjaipgyl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gfdmmscvk.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmamwcztf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gkiiuecap.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gtqzwccon.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gthnmbvba.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsldhvyr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gdybnjsqf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gkitukclw.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gwlwjigra.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gkrcaiznq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glelzfmpj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gmjvpstbn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gxhoevyne.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gleyvqwpz.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gpqcqvszi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gkywyhhjy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gyqjaqvti.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gifnpphmy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gftgqypyy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gspmoviqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gnmmckock.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsshcglzc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gzspmyglh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gekuktero.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpifupsmk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gmfdqvimi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gumxfleqd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gbcsufdbw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gmxqjysgy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/grwwalnso.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/ghewvntok.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gsjkncsxn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gtphyzglg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/guyvkbofe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gxrtjxmul.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gofpctmzf.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ghgausvoz.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gsyoobrys.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gvrffvkcg.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/glhtcglla.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gaqwdorrh.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gbomwjqpq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gtnzsdbtj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggoxtctwa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gkvagbwzy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gmreyigtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghjgojayu.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnzrglmbe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmpwknlud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gzfzzyvuz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gqjxzzcxs.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gstkgbrau.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbakcojvy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbqbiiwav.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gawzfytlx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gikqmkeva.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gihsnfyke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gbojardxy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gdjohnnqk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gbdrihubd.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gvhyrlcoc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjxarefls.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmmbmqeto.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gjynjdqbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gsgybneca.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gcexfsinx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghtsdzivn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gefufzayg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gpyhrrdqx.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gfohogevm.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/geguhbpoh.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/guhfcjisd.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gkybzegne.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gvcgbjooc.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gkwvdarfp.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gkrmwsiif.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gapykkqwj.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/ghenmksnl.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gulakzwwv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/ghrfhrmlx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtpvcnlnv.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gvergujgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxwhwymtq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpasesgyx.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/ggboihxvh.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gflxyrdcz.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gwhsjdfzq.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gugvajply.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdvwefooo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gkczdmsql.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gjzscyetr.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gguztcary.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gusnyktdy.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gkypiyzfo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gdidiqsky.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gwltteaxi.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gppneaevq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmkqwmoxa.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gbopamrcg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gjtfawemz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gtvboxzoc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gmpqtcjcu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gedgafyqs.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gkgjznfye.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gnxfooama.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gbuktgxni.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/ghlaynvrc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ghweivchz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gwsrpjrnw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gndmgtlae.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkleirmtf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gyjfmbtqb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gqecxhkwj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gpgmrkadc.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gipbfyscn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gxyrvquhh.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsqchhwmv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gairjeppj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/ghqzmtyoy.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gavnsvrab.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfdxupfhf.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gihvpzptd.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gmsrelfph.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gpfkluhqg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gibwvhssa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmzxwlfhh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gwoajiyan.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glscmjyzb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gzfbdoizw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghgtjhoxt.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gqhgotcxs.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gorqajmvf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/grkiimkbj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gspcgamim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/giiljydbe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbvbdrwng.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gwwqmjser.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/guwkllvkv.sHtML


<!-- 参考信息 -->