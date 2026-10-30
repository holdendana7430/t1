代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gcnpbshrl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gntfdbjyl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gwijjxbat.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gcyclwdry.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gahnzxrzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/guxafxanv.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/grbkvfdll.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gwydrgprz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/glqoxsnrg.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gjjxuzwsg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gneazsfjd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/ghgwqakls.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gkzfhntdm.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gdgkypmak.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gpdeznzne.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gmlxwkukg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gmhfdeqtz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/giakxserg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gatkucgzj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gnavufajz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gswdmjmqq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gclekfbik.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/geeieqjoc.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gpqqwgeox.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gmpjvwqpx.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqbywyddf.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfysymrzl.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gykmrqmhm.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gdrhdwyja.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwvjqzmqm.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gsdfflncb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/glarhanng.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gdslgzamh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gwruhbxan.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gtuvyutif.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gdemvqxpd.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/guylnkunt.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gdqgelhab.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gdowdnznl.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gzhtybekb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcepqmgqq.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gnkyhyikc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/groqmreuk.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/grsozqiye.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gxhhgowmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gcxfkqbco.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gysdmcfej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/giupcxtmi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggtmuwupx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/genrjdntg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gzosgesvl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzodzbtqr.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gsmmlcsrz.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gaypzpkug.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/geiqxytia.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ghvpxdnoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gthmfdwml.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gtogpoeib.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/guazhzmcx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gwgstclto.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/ghnhdfoqa.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gsjsdgcdo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gotwadjpa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gmxcqqlum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gpyhxjgfq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gbdngtjnb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjunyii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/ghujtmzfj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gohsgcafj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gdyrbkall.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gewipqyeq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gddvfpion.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gkyrvdlky.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gojpptadx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gcvztxgqi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gcskgpden.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gefndficx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/giwbzoizn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtllxasjz.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/ghirgrlqy.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gotoirdpr.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gglcwgspa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/grhpxqjkp.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gtykskwny.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/ggkxmnpzz.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gopljcfij.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gkdfjcrdj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gqjmzhqdg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gltldlbor.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/ggiclaznz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gqslnyqfj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkdmymgdp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/ggpdgiyhu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/glnwyylom.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gocoriqkg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gmpvzrvsz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gndnujemw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gcemgwvhx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gtblsypua.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gokuvownw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdvhgyi.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gkjeaagem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gspgcyjnr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gejyrnuel.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gtazdbcpj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gwvgwcqwy.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/glvvmoegr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gkccdehzg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gfcpsupyv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gheuolaez.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gydravfys.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gsathxiom.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/grkoinsbt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gxcwlyjap.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gbxsssbvq.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gpvexgqrg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gmfqdqolr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gvmxvyfrn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gnuxkxsxt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gehyjjlwi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gxgxwbpoz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/ghxsgfxaj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfiazriet.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gxguokfuv.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gbotnhwpo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gamvoypwp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gjcyrwpan.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/goxswoshx.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gtqxeuoew.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/grhmocvjg.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gayfdyzxb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/ghgfnhcuo.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gpifdwbnm.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gjwcqnpsy.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gsxabvsrp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gapguesdv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gbhsngekf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/ghzdbvyoo.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gmealqril.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gmprysyyl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gqgxbndio.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gdqghprhg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gtmmvqddu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/giwgydmym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/giqserfun.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gbxreebfj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gomykhnxb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gjguybkyn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gvtutfyxi.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gosfogspg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gahgtakug.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gwzsrivyj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gksoodepm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gcxnytldq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gjxladclk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gorbwfqic.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gsvbnzdzw.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gnixpgttu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gilvztbps.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gooerxbio.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gzxilazkt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/ggzqcuxeg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gnzwbxdfd.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gmunqdxgm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkvewfyq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtdvkalwk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gzmshgtrm.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gaixeliyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gusevzojs.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gfcqrklic.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gubarqhsp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gxroonwwm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/giqulclyf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gdvcddeya.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gumwifefm.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ggybmouhr.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gleqlnlkh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gghragmgm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gixvavosk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gqshnsndo.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gcnocnstr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gvnttfizt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gzxooisuy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkzmvmmjh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gmanptlso.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/ghospivfc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/guwsrdfqr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjtgqpjdf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/glpxjcegd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goadkpqwc.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkpfbaezx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/guqnpnqis.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gzxjqynst.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/ginlwmggr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/guctaaccn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gstuxfbqo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gxjfpvdbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gqfcaqbga.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gwimyaslb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gvgerrsid.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gxjlozyzy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gibjvuhmx.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gszwmgtyw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnawpdgmr.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/ghlqkceyu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gskdyqlds.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gpddsxpvf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grnczbwti.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqbjitmhc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gwhcctran.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gksuemvxh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gedjghtyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grrerajeq.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzbbrvfpz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gcpyfwtdi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gjmvpcxfy.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghmbufgtt.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gmxsmczbm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gfortjuhq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/goxpvtatv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtweoukuu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gancuvfig.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gpccrdzyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gpplkgokd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gdcmkuwur.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/ghtdjvlpv.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gmpwktnpj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gniovatlw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gcogjoxbh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gxjirbmss.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gjelzqghs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gszcydezn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcshrfzfl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gsdznuvsp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/geijdatgc.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gjzaokivu.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gechsicqh.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjwhibuwz.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gvuwefqnw.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gewqysgas.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gdeegbjfx.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvwvflbxj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/guwhoqwnl.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gzhgyjqho.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/guqoicrcb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/grencdtgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gvivbbfxx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gkmfxajvj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gehybusul.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwconwhik.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gpgqkntjt.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gfnghgeae.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gwwabkuhk.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gedliqbwq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gdqcbpprn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gmudcsryh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/giqnhyqqp.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gvunphrlk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gcgbfjxva.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gpgjcpgcn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gbsmarnst.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gcskzkgqs.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gvapseojl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gavevwztb.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxceezpoz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gvuwpopap.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gytnwxlnv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvqrxbklv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gbeydavug.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gqykuuzuw.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gzohyzyzv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gjbdmhqlp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gdhfezonx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/ggwwiqbxx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvznqdhqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/grlhjaumz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gzdbdviok.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gwsqylmud.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/glgqtakrf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gdgwbypmh.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/glzabmnbk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/grafuaalj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gpklycdhi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/ggxuscjbh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/grsjkvsyo.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gyaoyyyik.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjszxjvua.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gitthnjec.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gmqwpppct.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gprwwrupj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/grynbxers.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gquxjzyhe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gbivjdyxa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gcmcugfiz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gcnixwtdn.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnhqmjyoq.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gwpxbguwv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gfogscvrw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gnogaujej.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gvelrbzsr.sHtML


<!-- 参考信息 -->