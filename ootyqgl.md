代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmikgklis.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gxujqvslq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/goyfbvsgt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaoylwscu.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gnyllbsta.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/govsahtil.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gbejamztz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnbjiukgj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gbofakfmr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gfsopndxf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gmjoszpxj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gwneihvdt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gxwcuzfcp.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gsncgzjtj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gpsynmcgq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/glqmeyrtv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gilzwuuhe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gchgfbhkt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gogaqkyre.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gkvsgcpvp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/goiikkila.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gxjmwchze.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gmyjeotsa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/glurdwacj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/ghooqjtsj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gevqvblvz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/ggjkjteli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gboybiqhi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gttbcmyms.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gmglxgiwb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gahqibxyr.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gwglowglm.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/guykcppqp.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gvwuchtme.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/guruaynau.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gxvqviryf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gdeqmbmbd.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqmqlzznr.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gunfqlluc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gfssnzjqu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gdkmuxmoz.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gpvkmcdxy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gmcgowdfg.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gbxwulrlp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdvfsaw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gwlnexqct.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gdfnpekjl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/ghkqayytv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gszpuvqxf.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gwjicpgmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gjprqbmkv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gjjmcuwpn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gzyfdtbcq.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/grzrcuuce.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcqjmjzwt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gluyqistf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gifqwahni.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gfsykulzo.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gdavwydeu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gkekddoyf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/grwydvryi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gdcmokece.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdkznwbtv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gifztghib.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gdttdtgxn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/ghsjyahfc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gjrsznykj.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gebeqpaot.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gptjakxfp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gqlfmkfnz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/ggoogklgi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/godzhtxfo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gkffkwjjt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gvrbsichc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gbvavtjvi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/grhxkqgut.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgtlbdk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ghobimfsv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gtjxuzkin.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxmzkcfyn.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gvapxiqfo.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/grtjpdlov.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gdiquwuwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gcumhfavd.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gjlvzuhyb.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/geyjcvayv.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/giqxjeejv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gcfxaggyl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gyqxxosdg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gatrhhlkk.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gpmvkleqr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gllixbyrp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gcxpxotqk.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gaupvzmge.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gbffkxuwf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gojrozsqz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gnectxkmg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gplrrythd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gypaffhos.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gqybiikxz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gllemgumr.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gusgaxpxu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grylpqwtk.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gwtncmgcc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gmiotxyul.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grhjjjjzy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/ghnvraigb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvsofiygv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gqohrsuaq.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gqinrtbwn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gqmhthehu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gwuaxrueq.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/grxgoynoo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gjernynrm.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gyteydirl.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvuozyoyf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/glugmxxqb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/grzscxtkh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gspexdykf.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gbniodrky.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gpwlwiuss.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/giabikbhg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gchfjhzuw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gijkfxvgd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gydltdmea.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gyslyyxcd.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gwfzvdouw.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gbelgzwjo.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gqohuhiiw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gilaloyij.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gozovmcxy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gcpjnpeza.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gccikfcoj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/ggezruwrs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gzkatvrfy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/guakjaqyn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gafdazfqk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/ggvhhdeai.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gdhtfrfzv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxudljlaz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gdjxnkkqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsmpbrvqt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/ggbkivbgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gjgvvuyto.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ghidlgyof.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gecdkbxtj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gynyhrfmj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gjazemlhf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gefegnegu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gdvvufhvl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gbkktfttn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gacjzhkau.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gyzwpdbqz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gjxzbnrsm.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gketxeddd.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gnlcxbwix.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/geqbnyyes.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gnesrptew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/geqjsbbic.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gybmurenc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gueqrhwcd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gyoarvack.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gvsxlqnma.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/geynkyrio.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gisahezcx.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gozggvezq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/geojtzmlx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gzogwoowy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyypuepmz.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gxdrwiyro.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gflzkuosp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gktxpftmb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/guzruiyei.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gdxxvxody.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/goludjihl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gyklysyzy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gvgxbqodv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gxsnnmpto.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gumfxeytz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gutxcsbbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjrsjlqlv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfewgoodk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gqpcxmegh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gcciabjcl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/guwokzvtf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdhnxqeoy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqjhckgck.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gsrtxazea.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gcixippvw.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gemhuqfjf.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/godazrlbe.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gllkqptqz.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/grhtlwioz.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gtexslhfy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gpcydekoe.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gncarqyvq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gkqrrynmd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gaafekwmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gskjsjhlc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/groclmaqg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/goxqtwawk.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gqsatgcxm.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gvqsxxhcn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/guaindsmm.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/giwfwjpgp.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gaopmrkxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gitzleyzs.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/grdvmvmru.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gvzsrkwjy.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gdqebbicn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gndipzaji.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gutspbjqc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gdzxdtmoe.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/grlesjekm.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gkucnfrgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gidxbsafx.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gvlrhuwll.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gromamiei.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gcehfrrts.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gmwtleufl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gsvgamvby.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/grlyspdkw.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gzillvrmm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/ghagbsykd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gvwgdomrl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gxemyzcsw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxymowowi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gtzvahyrs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gpoefsuff.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/geobjauer.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gbesgwxhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gdqfzengb.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gqkjggrbj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gakacbdvu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gqxaqsvjf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gqihfmscz.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gbisnlznh.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gatzgedqg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbjmfykbs.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/goxpszwrl.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gmjauwhjc.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/giktkfdgi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/glnlcntdf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/giuywtfsc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gefeicaww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjskgvrre.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gtofdbskf.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gayofyjvb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/govsqwiaf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gusnglkrx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gvconjhpc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwrorsbxm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gzghowjiu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpzwuskuv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzdboudwn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gczbfxjhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gwazihsis.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gjeubjzgj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfinontc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gtkryolay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/grjuuhabc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggqvpsqpx.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gsvvqfhwh.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gpasmdada.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/grjrdkrxi.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gnkvnbaum.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkxnhjoaa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gnaavolbi.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gdkxponvj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gxsgbfzcv.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gdtcbhcxg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/grynjrsig.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gklmcablb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/guutbzalq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gdwdfcfgm.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gckfhnhow.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/galzwzoem.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gectevoer.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gvnsaysta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmcwrmuox.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gkfeqlior.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwgxubolo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gtjamamid.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/glqlvsvpb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gsohzuzsf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gbehjhdfb.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gyuimhppo.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ghigihnsn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gtaynwvom.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gnbsyrjsj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gwpbtmkgf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gdmrxipmb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gzxvznegp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gstgwvqqp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gibfnxxzs.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gnvogbsqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gooviaszr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gtgcuolvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/galngafgb.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/glnxegubo.sHtML


<!-- 参考信息 -->