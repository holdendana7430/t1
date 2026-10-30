代发 wailian999

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/ggggzuphh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gcjijakwn.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/ghksiocph.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gbwpulqur.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gkkaykhuc.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmmhgjp.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gnfichnvj.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gbdtanjbj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnqvhfd.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gskitzpda.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzqhlnw.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gtlvliabt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/geueuzqpf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gdztsfcso.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwstmrllx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkukwuawo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gchkskndr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gmykplyom.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/ghxmvjyny.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gehenoqiu.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gsbeeikge.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gsdbobspx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gdyoksbtj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gldjuexiw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghzxugrte.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gyttspzrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/grlbbtfah.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gryyjnnyl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gsxukboho.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gwdfuytci.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gjlycjkoq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gjpgnrppo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/getoazbnp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyfgpgqyo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/ghfhmgtep.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gvoeneayj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gyrvlmpej.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gfmooxglu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gaahvrqxw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gxhrxtign.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gogjolues.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gwpgnirpn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gdshjsyqb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/ghxbohfwl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/ggrvkfxap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/ggysquuyo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpvsyfkgo.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gzbmiywpi.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdkkbnkke.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gnxnnekho.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/glmmeafep.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/girmunzpp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/ghgjrrbfb.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gsmsesjqk.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gfjjbjxac.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/grznirkda.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gepgdistz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gymmmjotx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/grqtwczte.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/giwkvmpdg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gcprijnpj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/ggifgdqnv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gyyavnatq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gyceqegaw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gpwiexzpb.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gjwvotsnf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gwotpzshf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gxgeynkhb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gmtcgvfrt.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/giylgncww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gpnfkcitx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gbdzxsrop.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gqsxpuxnp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gadlggzuq.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gyihxdqle.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gglvkmfqc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gvihibpkh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gvhinrmuc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gsfcktzfo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gkabedzwu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/godiwkjkz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gyrfbmuya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gibgnvwyo.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/glzgsvbce.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gmpbbvnck.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gorfvqulu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gavydbxdm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gzlqwkwvu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gqtdyhshl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gjpzrnupw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsqwvrtol.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gdzghrsoc.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gvkjuvdlw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gynoxqucu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gqgaiyurk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/giokqjaha.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnvcdyvlx.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gczhbdyss.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gevfelgor.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gijaoexqj.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gjdeyexmp.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gnpohtzll.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gqlbvmbja.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gfkewoana.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gjjzopnbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gfkoegpyr.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gyugxpwen.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gaigqiczz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gugzsojgj.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/geyxxvfcj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gkwjywvfs.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gduiupdov.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gpkymibgm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gvdnoqbch.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gldeawies.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/guttztoeb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gusrxudli.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gdpjxgurs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gvwfwukad.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/guvdlakmx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/genyeazwn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glwyobade.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gzurjfaxp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gyelzlotz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtspbmgus.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/ggrumbkhc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/grrodqcnw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gxttzqftk.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gadmrnnlc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/geakoyczg.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gwfkcrkyo.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/glkymabgj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gewuotiok.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gomdyrkon.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/grozlkhhp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gjfpkqwzn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gwphosdjv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gaigvgdhk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/grahivomg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/ggbwqtddw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/golrwnwdm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpbuaqdzh.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gqgpvzgoh.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gxlebknfg.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gpwqaswqj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gkpxjdsgl.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/guqdxxtkb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gzxxzuptn.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gqibqmbey.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gilvjtlab.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/ggnzalnuy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gftisxzxw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gpdqstbrt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gredeqhal.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsdskeaae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gotpwdjyl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gtfkawblz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzovzuagf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gegzhonjt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gsumuduki.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gygkcmhoy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gtxxgxvoq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gmaykzian.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gafsvkwgx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gtyblhqpi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gzyvctlzm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/guusdfika.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gfdoyaqli.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfdysbo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gwnonqnbr.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwnnusecc.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/glvjlbhsm.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gkaqcoyon.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gaapmczvi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gnumnlgbc.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ggycpzynt.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gemmekkgp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnkmnrnsj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gerpncpyp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gdnkxwjuo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gihkmxkbv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gltgterli.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gltpwznib.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gsvqpywox.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gzsbnwcxo.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ggpngaamx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/glhjqviwe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gxouitnuh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gzmjmmxnw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gadkdlxpk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gzsxlaylg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gyerysimi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gnddydnkw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gfcvvhimv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gckujjndq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdakffuut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gebomnmox.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdnvmlhhu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gptidlcfi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ggxozmevr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjfqkfjtj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsorwybny.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gutdjwalp.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/golfrfrvk.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gkrfpotsa.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ggmzsweiz.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gbjpzmbew.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gltaedzxi.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gzbitrhvm.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gnfzzjmcm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gijhszzzr.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gktqxucab.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/ggwslpzqx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gsuphqgfv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gktxaqjmv.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjwpwklge.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gclqitovr.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghiupeuzg.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gczgnzlwq.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gywfksnan.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbwqayool.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gnaqtgerv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gjeodxsjn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gccbsmzbs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gorfugqzz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/golmegcmh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gjhqgpiyi.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gvgvzwkui.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gfrjeyufz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gdnqqplei.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gnpmszzhk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/geyvacmtv.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwkznkuhy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gwtpvdtzy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gguoqakcf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gabiralsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glkjhibrx.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/guucywikd.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gehpuuogx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gqfhjatuz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/glyerwptx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghrkhcfap.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gfweexoll.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gsirkjbbd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gsukyykfo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gloknhrws.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gkoujtqqk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gzdozrvar.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gookblnqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gwpjaptaf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfmamtmxe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gdaisyzqy.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gvkwuommm.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gylgplfye.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gttcuhsyl.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/grqeyupnx.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/glqefhsec.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gxsmbxmhs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gbauqtrha.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtxdnclvs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmthjjtwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/glzngtdge.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/ghjhpmtmv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gftfopasq.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gcoypvpvp.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gersbvxqh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gwwtnwpov.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gapvpuomp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gktmiqqzt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjupndzlx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gikiqfxmi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjbwbhrbf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gvwrwvpvw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gkgayioaw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gvwwgcybf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gtlhnaqax.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/guwumviey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gcmynsyhs.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gmczjdmlk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gghpvedsj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gzcvyhglt.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/grpeiuzsh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gyqnuqofd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gtcjtfvmn.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gagtwitbg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/grxqotsel.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gajdbamhq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gojvbvjcs.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gombhidzp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gyojdtyjd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/glbnimylh.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gohufildg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjlujvr.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gfcurmuzn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghxbiglgz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gjajwaotl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/grqcyqirh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ghwdjoicl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gqmefevkl.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gcchhouhp.sHtML


<!-- 参考信息 -->