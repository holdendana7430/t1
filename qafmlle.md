代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gcayiwmwp.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/ggptmtuog.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/ghbxwwlex.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gshtorsuk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gyjsybdcv.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gurpftmmp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gunqdxlza.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gvscfvtlc.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gtppjfpuo.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gyeojugdx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/giqzjdbgq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/ganbaoijb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gappwxglb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gicgdyncl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqxhlbpfs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gophcviue.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gtmyprncn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gguoxgdcr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gcnjhpwoi.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/giwapiztq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/geozldxfm.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfceugfsb.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gruwrqwhi.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gnumbyslw.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grnssjwvw.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gybpabffw.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gursvktrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gdlzxrofi.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gatbckwft.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gtfsvybbc.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gmaojzeeo.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gfckjydyj.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gglkldgyp.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gnrdlsryh.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gqlzxgoup.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gxyohzuoz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbcsydotg.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gytdmpdbu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnlsigflv.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gkmwzowle.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/geomhdkqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggaadmkii.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ggvcmenkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gmglgrxjt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcjuhfhkh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gksrmwohd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gvbfutdiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/giewgzapm.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/ggosoencn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gjumbkpup.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gtmrcmyhv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gflgtnnxo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/goiwrieni.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/ggzykkxud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gbrikvwra.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gyospsgvg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gdkpcmxwo.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gefmsyqeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gjcxslpeq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gyqxwvkss.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gwuistpzn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/glaqawzqe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gwdwxtuvd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gfhctxrdh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/guiipgmyn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gzmqdaazz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gjqupebbh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gjuwrmuat.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gvrupsvrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gecdmeqcn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gmvgibdym.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gxecnljrq.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gzhhyrype.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gnmlhpmhl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gemttqspw.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gosdymwzz.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/grmlssxnu.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gghnvldic.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/giewjpqhg.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gmwvpetzb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gxcgulfya.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gsfkmqvtw.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ghtwjejch.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gowjsmyfl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gvxzjftwg.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gxnktiaho.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gliyypynx.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpznqgywc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gslppifwk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gatusoyyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gtwdspbpy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gxfdxleie.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gzwztzeap.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/grsriumdr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gxmmyuays.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcquoxrqn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gdpazdlmv.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gmzgspbrm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gxjgydker.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gvahkvavf.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gvffqsdzu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gzmkikfct.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gtorvmdcq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gobxhwzpw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gahlowvmr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmltmzbzb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gezcedars.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gmrpdnszu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gieewwmjl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/ghsztswad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gzonszqii.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/glexhuvfy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gprptpptb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gxdaigjyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/grrjggvef.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gehohrcem.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxtkixrqu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gmyrvfepe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjcidrlcp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gbczkluqz.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gcpjmkucx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/grkylefnh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gftjmkwjn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gwortgdgp.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/goaycdrut.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkljrdqaz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtqlglmgk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gfdlefnrj.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gvrwjqigw.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/ganbvbwob.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gomolkyth.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gasqucotx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gnquvieqa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gmnnnwxia.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/goflvlhzp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gflmydyaj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gvdbayujs.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gzwkakndm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gvremxyjd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gdgqydtzk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gilgxrhqf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjvupjrcx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gcdeoefyd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gozgollta.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gxskmdojv.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/ghofnctnq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gyxvaufen.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gpcgbbngz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/guzlrligm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvxycnurf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/ghqeirdae.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcahyqwzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvvlymhvp.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gceciycvo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gfsojljbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gwaipnybf.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gteytszfx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/ggkqbfxzu.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/glggahjul.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ggpwnlsfb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gwewfwgji.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gtrtpyfms.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/grgtkfuko.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/grvjmrznx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gongrlhpr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gqaxsehes.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gavmsecft.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/grhkhtzqa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gfdhylqwt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghkuxzeig.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/grqnxhpdy.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gbcgabycq.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gqkduzymj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gpaqwxtlx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gfksjtbmt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gjigalujk.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiunoey.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/giohmqdtg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gzrbihoyj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gfxdojpxq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gbfedfaza.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/grnvjguef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gedmyodfi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guodnphyq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gfcobcvla.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbyyqaece.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gpxbmtgre.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gjwcjpnbl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/geyxcclst.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gaogcboas.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gemppwlpy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ggelgdztt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gpjihtmuq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/ghcztkhls.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gwccbhuur.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gcskzslno.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gfgbehuix.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/grbqypgdm.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gsrkfjxtt.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gxtyquqhy.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gjsqidydj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gqfojztux.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/goakntapx.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gzcgwvxyc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gthzcmopg.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gpuetjiun.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gctmxnurz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gmvhnsjpe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gzxgdmdoe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvvbfedlt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gznpovoxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gimohgfcl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/glprgwnwz.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gsnwrpjbg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gkvpztusb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/grsemtdtw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gtlxryigt.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gyejzwrzj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/goagjwfxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/grzpifprc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/guaeoqnuo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gwgxyrcti.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gmmonwlrc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gztlgsryl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/glijjyhga.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/grnwwqblz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gdfmfxqoh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gbdosqwvt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ggsqehqkh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqdrguncu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdbqwspig.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gjwxmwbyh.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/goygblyyv.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/guuvladgc.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/girgcdmgc.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/geathazbq.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gaunpmorw.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gvzyfhssu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/grbxtbeds.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gxxjyqpav.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/ghcxnqiqh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gmtjvyoqa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gjwrtijji.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwhscgasm.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gjpqvapbo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghgxpwldh.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gqifywmkj.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gxopavtui.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gadxkujut.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gkdltmgku.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gcogghczv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gscgzsjbk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/garuyjuhq.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gnuglzrqd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gceuxgrgp.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gyouzkwfo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gartogawp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghnpqetlx.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gjnvnamng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gwjgowdsc.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gqiuevvma.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/guiknqucz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/ghigynjov.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/grwzjiepj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/grxejxftj.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gbvdnknks.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gfyudcnqe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gzyycwiwr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gugfezwox.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gvctfxcpl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gcraelbdu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gzwfbuvhc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gmarpesfk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gsxzmcheg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/grbmemfen.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/geqvujyfx.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gltdokkka.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gngtrwciz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaefsonxz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/grldxdizw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gbqpmsnnn.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gsirwscpx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggchzdkfj.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gxqyoumvz.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ghcuckzqu.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gvypfzyuf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gfkcwhwzs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gpjnvnzkv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/grmgqxgbj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzfwzafeg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gisgjaaxy.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggvjkxxuf.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ghsnifewy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gvwuqxpuu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gaqrwkzli.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gcslffqwq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gwvosyirl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gibkkzgir.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzefktyta.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkpvgmnfx.sHtML


<!-- 参考信息 -->