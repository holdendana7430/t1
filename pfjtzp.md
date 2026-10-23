代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmozuihj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvheuodw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3okzrgrwa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3grubguon.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qwfpwlsv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xmlacqog.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gmqnjooa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3unbjbjyp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjepsbcb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kfgudazm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3whkewyoj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ysilydbp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dbbvwhhk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ramqranp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lwovujvx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iyzkivub.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pbmyrxwp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yfvvofpu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zijbqtry.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jycouequ.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hepgksnt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ahchjfqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmxifxtw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hyrxkoxh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kkkklkyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjuaarzn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytlyhzij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikbfcghx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcwdnej.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cutegyai.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pdqvruhj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dkobogkq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmautnha.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3odhxtuax.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeagrnrt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojehvzlj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elfagzir.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bywvifdc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bhgpfdkq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eqnrmrsp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ebvxxkis.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jaczhulp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gcsolizo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oodkdnco.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rciwrxfm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkzczrz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rssnjvnc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3alepkqht.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3awkjjhdo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zaijlsqf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cyfoqrcg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ynzxaeqb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnthjriu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xikcyyzo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wbsmtvxi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fiswwzba.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkxbtgzf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nyvaivcm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqtjbti.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ardsauzx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3aggsnrpb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sdgkwaif.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3naiwncxw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wzbntqtj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vvjdmkyv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vmtptizu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qejxlrnp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vndtuisv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qatedbxc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kgnlobuz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tcthqqes.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nkemsbcx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lhoaedrj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rheiomay.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mxsfyese.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3oskjexlw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dljogstd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xiltwobt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ceavcykj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zuetcibv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkdgluy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jvoorukk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zioqiqwz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ohuozujt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3skcbzxld.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hpgiubse.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lurdzcxh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3moqnqqls.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3catzmmtw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aopoywpl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgnypifq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dwjawwkq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mpvdfsmh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kjroqvbf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ismhmdsu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddgqekhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtzvwixa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3oclcgofl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fnlmkmdo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qmznpamv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3baponcfc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3izluvklt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibwdajwk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jogolvgs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jneqmtpv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3czvxmfok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qvlgpxsu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nazzcjuc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fzxaihao.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3acpllzvz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zvhxoynl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tewpufjb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3denufmet.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tkxogzzc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wusasncy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wynblwxn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yohzanhx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zawimfio.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qyrcuylg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rkvehjfr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pkkzmeor.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mnmzswhw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nnwhrtro.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hcwpbclk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3udmrryrw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yqwnmomh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vgtsaoqf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yjqbdwea.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qvhccgmr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kdirdwhk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ybuvcerk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nwphdscb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3urtxtphe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slafxfsu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3esdxozbr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vzdhtuzj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbivrxtz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cuzxmsmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pkgecpnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xcdzgabz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3iwtlwdmk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fehmqudo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pxtparks.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3shkrfnxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnzjeyyt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ayknhfln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3swavayrx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3amwrmqov.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kbjspnmu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ggjzlqpg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jkivzsoj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wojhjzze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3adhyzpzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3axzzupth.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nmhacvrl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nbavnnwm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3twryzdvq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xygdqudr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zxkgwttp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hdspudum.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rllonbxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wguqixyt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jbxrxdmj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hbgcnqvh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ktbaimpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmwknluu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hhpqduug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddqjffrs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nlfrvnrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehoordkl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rqbjajgb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pzoqqgmz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yopbgcqb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gyikwuxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgqkap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fojzulil.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3biskvluw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sfgnmwvz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ftlsujhv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eokdbarp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jwutiwhm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3emfyadob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uzzvtnbf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uovoaeen.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kufuenaq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cfknwhyt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nrypnvee.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvckibl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3eetxaacr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwyiewjc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdivtwen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3oyxuimbb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sajzimbo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qlwbenmt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dmaudxhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3slfuhbcq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tpdyeapy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmaivrlx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qngckpno.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qrcbhwsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bfmbhpin.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mcmbixqw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxfuwnt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3byvgkplg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3emihmskx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hvjuvjze.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sohqcoke.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3octvwakv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvqzmoqm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lszjcvrn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cshqoguz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jrcycwmt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3idxnpjzw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kfsxhlmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mhiougci.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cechwrqm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxovvkhb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xqrrnfon.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mvclbqns.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejrnniuz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3svrrpjud.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjulqiwm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yorfrbfh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3euylfemi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vchbvuxi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ndgzakja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fqxpnkll.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nwsqmgnl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wtjrritf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhmddysc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ulirsgjx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wyzqcfxm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ccnhewsn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hugnjviv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjkmyzr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kaaqmaqv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wbjhoyox.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3aybwsppa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rwnnbsyd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nrvbmxdf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvyprgp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ommmjjdm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bwcebbhc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jfukekeo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lmqabvuu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hepnbumf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rrxmmzkg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pnhzammo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qivjeyyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3izkhegja.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eoxdxflu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lzowlrlb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3twxkhzlu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vzqazcdy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hgmupzth.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ufrxyyxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3utozhtyp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3emyvtldl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aegjlxjd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hipuqtyb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3eyiivhds.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tosmxpro.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3snnjbgpi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bfmjgbnt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wnnaukhq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3znqzitxr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvkgypou.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uhasffgk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3surduufd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3strsjatv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zaejxgxy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djifvylv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pjnedlfj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3smmtfhzh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yszehylw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yauujoxm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ungjqjro.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3leqvgiri.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ebpyjahi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xlxaymyj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wvqnzzjc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dnwqtdjf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsmjybk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ffnhqdwo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bszicwof.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lhqovabt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pupbeaul.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hyamcasi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jqmneygb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aprgrfow.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ojzqgttf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjbczri.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bjybtgkl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3arlulkib.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ufjoiatg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wjyyvgqa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uzmgumwl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gnoindto.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3semqvtvl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dhcouxpo.html


<!-- 参考信息 -->