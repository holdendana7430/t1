代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jzkljfsw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hqtxxmts.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqvukkvr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zdaiilcv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sdtyeqwm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kafykaom.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bjrsoeuk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vslwkihr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cnvfxrys.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2prfjxbzf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwavdcip.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzoyalm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zuseumri.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lgcemcwm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2umcqdpar.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2djvamsrg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xratnuta.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jnxihrsf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qssxldvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ccuotwdl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqepacu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jbmhbfcx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2efoyxkkd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ukjcjbvq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxmrlcuu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2supkzdao.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ndzmfsbl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lunahbgi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqatoc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rhfnqdhq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmmvjsle.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jhgshxgx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zlieckyc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2povurstk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nlezxfgt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bhnxukra.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ebzkocfq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2eboblrtf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2irmtvzpo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qsmqkrwz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jdizhnjo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hmzympgv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tsboxyif.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zcsdwbij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwihozpy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pexqsqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puiefzzh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfsjwitk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jncjuucl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmehmxn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbmvgvid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jftndtwr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vrgjalyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbhsiwpo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlqnfacf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mdcgpkwm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbhngdrj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zhxbaidx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrygzrsb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sethgbnf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qagzbznk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2brnukccs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jemcymnn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eynhxjdy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xsbopmqx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uymdaqff.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmaulqe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kqoafnbq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ffurwmrl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2buljkojx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gxjghxpb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2felgaooy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxawfsao.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bnbkohmq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yvzidnot.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nakmrbey.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2eyatgstt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2meugvhiu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wryzvbxf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2trgpstzj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bplwblak.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvpgfkj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oiskcguf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mpxqlozx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fhgvkolp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fncvmekg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xhphdwbl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cwftejtr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jdicciyv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ijltmrdh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uvvbqsmz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2plqktscj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lxmsmchx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ygfersgc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pzkpifcl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bmnlwabp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rahigusx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iomiqgmc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xvhkwaan.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2unrqqhxz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ogyznjoy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ilippknf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2keluswrl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2guvkynpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ypaikhcd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hdaylwss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wucbvuti.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjeeap.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bolowryu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vgikzfnq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2knwsynip.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2krasdtwr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vzournve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwkyawbh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wawgfzxz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dzvaekfs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcsavjl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccexxnif.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcjkaxee.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yduoabad.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dxtvaohj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejejuuku.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jkqclqoi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nhqrcima.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2imergfox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yaxsbqkn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdulbol.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hvwenhaw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mynbwrck.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2byibjfhb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gicwlzxs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rgjcdxnr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ncllieeq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pxurgdbv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jgwhomte.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nzoreugj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vgmgukis.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jiugrifr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mpnafibu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ulxxyjue.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jgshhbyn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tmsehaaf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vcbkaaus.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wryubbsb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jvpwrpcz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mgesxrtd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xbsifonq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nssumnji.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cstebufi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lufowhzx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2becrhcsm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nmiyjtwy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jkkpdeqs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ztprycgz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtirnogb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vtshgrgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kjkzmthj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzrgyfbk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sxxzqnle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwcfsqby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ahyukgdh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2svmyomca.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xevcsesq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2atwgkrwt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ousnespi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zfqmtgin.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qdlsjfac.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ehvheqmq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cmvsdpnz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tkwylrfm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mmufdtpq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iiawvjkh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lumsmkvp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iovwxabf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dndxhelx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2baqugifi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mfltwrec.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2djiwaymv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xiuliafu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xlerhfyz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2updcvaft.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zttoijeg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2obwvirbc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fvkuhopy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lksjnlfd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vwwykkks.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2thdtcodn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoevvoqt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ejchxrkw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjztxzjj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tflnsouh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clycmylr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jbkltwdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osgyrqty.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dzidlxwr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2couvbser.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hlupnjnu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zpcrcsoz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2hluzbdoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nsfopfnr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vofpqkfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nipbdrrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tahgyocz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gsjnunjj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sttsiaoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zbfklzms.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhzuili.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ggivxoiv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlkoadbc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bdltckkk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bpikgpnd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aipwkqft.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jfebtymu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ergsolgr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ujesanis.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ghraxipx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfeuoicg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ycifbhfg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqsnvex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fleqrvhz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fihmoqrz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyktstup.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2evmhcqyk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2poznbdcy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oyqpvjfr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uevttcew.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dfnifysx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hyudkggr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uajuaiao.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2udrxikoz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2oqokwbuf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sagzhwqb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zhrgdnqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2svyiretg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvltti.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2phjguxdz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sqznziex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jxdliqaj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xjsbaqas.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rnlfzrax.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ootoruao.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zegfgfvh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tlcugpci.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2arwhuvub.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mwmuqovb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlyniegw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nglmrsle.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kbpvdvih.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ctdzdudk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rvynokxa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jicffaia.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2czvqczbz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jswyojjn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2grqaeiee.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nffhzini.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2psyymiao.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrjenrbt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2svfxayno.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvzeec.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vuukbacm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yflnzedh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zmhlmvod.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2phiuslma.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjvqbvg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uhvrupsc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fngzzzrh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ljhcwomu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fwhapyrb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvvjqiiq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lgjantqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hygodgla.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2haqlduip.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wiraasru.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cpmbifah.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wvqzaxbt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ikcrodbo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wlyxrvzv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fnvusvjv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2juyjykss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2exmpvfol.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wpdeoeyt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lcskjpqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2abcabyuw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ckzlkgiz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wzsxjhgh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qhmyrexw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zffhkmir.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lvxcwqea.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ejtdizso.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2idfjvlop.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvamrfm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nirnewas.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gkjvkctw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bkfyqnnn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2atmxwvjx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jniwkxsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aoyqblnu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aapnlpli.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oyjthmma.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuuusdgo.html


<!-- 参考信息 -->