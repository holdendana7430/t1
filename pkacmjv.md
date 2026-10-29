代发 wailian999

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/glzakyajd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gbyxgvmac.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gyrgeragi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gncvdxphg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmdmkzhen.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gwjllacwm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gbcuxtkhr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gibxrdejq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gdgujeeay.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gvamweotk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gunbeosnb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gbfzazeon.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gtahreiru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gogpbtqqb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gfyudhhsp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gkwwxkckk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/grknvqptl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gibdwjtjb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gjtxhexlb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/getbkfsjb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gwljmdesb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gkdzlckim.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gvqgumgyn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gocyqfoaz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gubzmrqet.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghvxltdlv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gmmoxbghc.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gdfhgprgv.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gaxsddnro.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gcszuhvdp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gusycjsvi.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gskjkgbee.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gbtcjfgtd.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gcvukiuib.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gsbqbkpbc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gyicpcviu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/ghoszxjuj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gfrlbkxzb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/grhwuwuzx.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gpdrwtaim.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gtdecweon.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gjigocbgu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gpdupqzua.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gqumbdpei.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gijrsbymm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gmwfaiejr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gaafwjlfk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ggxgmockd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gcdlbyywq.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gzffbjebx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gfpuclgfs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gqplcltce.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gxikzbpdd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gnmitpnqu.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gihudurjy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdeilgs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gplbvwsex.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmdehywaz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gxpkusdev.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gmgxvizcd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gifctzxnz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/goisddbwf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gkohslirf.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gnykdotkt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gjqmvudim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gbzqmpmzb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gqkmjmslo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gzkiapqdq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gjxyqqrym.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gzzjmbaqa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/geyhurocp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/glakqxslz.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gojohcmam.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gntvylyph.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gsncyvowb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gmkwfazxz.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gaiynyjpr.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwswdnlma.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gqbijexuo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/grphtsimp.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gfzhugpxv.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gppwrzizc.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gdcdakqbr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gpjgtzhfq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/grbrzdujj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/geesqsokv.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gtqhvwblh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/grghrykhu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gvripmbpc.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gdgtlcfoz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/goifwhqjd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/glxvkaazk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gtirheydv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbjocbosj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gvhlxfhgk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gafcjbtnr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gnmzjbnvo.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gafpnevjj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gerpwrnhp.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gfxoeigaq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gkgcekorv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjoyqhbij.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gcjvywpkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxprkrfgt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gxvynqgey.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/ggoiumuoi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gqeyctsfw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gekmyqdks.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gtzeliygm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/graualojr.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gjurdehsn.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gkrdnawjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gdpuceswg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gezofncre.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzbnyezvk.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbsdelcvj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gwcvrwmrq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gomdltwef.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gtvpdtdjv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gjpyvggsv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/grbsprekw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gxtvvayjs.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/giqxdzxyk.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gjhhhjnas.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gggrromhz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gtroidgtt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/ggvsutzvp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/golujgnyn.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gjhqqctpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gropovfqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gytluvmep.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/ghgbzxavm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gwhbalupi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gzebrwjqp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gmnmprbki.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gomrrkxan.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gozfunihq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gruwbtuzy.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gigvdhfos.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gvatdjbyv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gijxixwjh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/grkkszsix.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gxjytktla.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/garsfoayp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gaxhthjyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/greiuhqmv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gvaevgzrm.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gzjofqbmf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gjtwhlkbz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/giehikfpd.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvjacalzv.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwaqdwqvf.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gbkhjjmxi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhtssew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/glcfzzoig.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gijfrsudh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gzgmutuud.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gnegwqjre.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gfyqthfqx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gwzdrwfdk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwbuulhyk.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gylsyoovn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gxcmrdtlf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gasfekjle.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbqpvxeec.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gmutgfhuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gnunrgfdi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gycgeemtv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gdxdpqogp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxckashun.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gqfopdokl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gduzzhghk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gctugeshw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gjaehawux.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gnnmdmhcp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/goqtfmeji.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqvlxfmco.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdyzdgbqe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/girbpodxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/guwcaimpb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdmhwqnzs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gbzjaiayu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ggtjlloop.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gazurtamw.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggsgilevj.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gvxfavjpb.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/guucrcdot.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggfvtdlow.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gtatmuuts.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gedfeckyf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gwxvbxjxf.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/geolnwqch.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gpweemnfq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/geyearzuu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gvurbxoxi.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqtgljgbi.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpvehktfk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfnptspjw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gtpwrdlgv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gpjlrbbjf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gyysstcna.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gvkyarbmz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/giqrlbfdo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gqghmjpbw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/girgzycyi.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gfvcvaqzy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghdodqxoj.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gjgcaromu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gzuzwpaqt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gabhjsedd.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gtilkeugz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gupkwmmnp.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/ghejzagri.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gxtfwunxg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gielbxbnl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gtqhkxnov.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gltwgzomq.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdttxwbsj.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gqavwvqop.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gzrwrnxfs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gspklxpmk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gqdwcdlkv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwdjvaneh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gsydpmufh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/ghuisajuz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gqnstdtdj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gjfsutuql.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gngyfaceg.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gmmspylvw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gxnoiuipj.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gkkevqpdl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gdlrhiinj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gubrqwyya.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gdikcjubb.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gpidhgwrk.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gqofjsogt.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gmcbvziph.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gzfytmrop.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gshyureiw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbaokplcd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/ghmrkwlxp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gycogqafh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gxiainrvp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpurwrqer.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gelfuucvz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gtbfohzto.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gnfogbaib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gnltdfwmu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gpxrrljbc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gknvcmrqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/glztabhiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grzqwynyq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gpbetikqh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gsledallm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtmubchjp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gsxitjwkv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gvpnlwyio.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gzdhpeohv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkrzxdulp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcuijyf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gumxwripg.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gvfpazlsa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxdrjhjag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gxocgdeqb.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gcigrewyj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gougjjwfd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/geqehibzr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxqcvdacf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqpbsmkzh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gqrcyxjbb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gqdxgnjir.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/grgpnnvib.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzumkrunv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gkfrsrfmi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gyrjomhup.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gymmeopnq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/guvoutscl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbbmpwjdn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gfcactztb.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ghicxcosp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gvttdpghs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gyaabqowe.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gjtvpuvwo.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gfjtcuwoe.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gtegxmuvc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gzdemukas.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggggncyqt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/glpixqylj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/ggklmcwxb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbemkhapt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gybcrldrz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gthwcgwrr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gsvwiqqnl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/ghobnpomy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gcmevgqrp.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gdkqbuknj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxtrmsiji.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/glsedfeys.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/grhkosyrf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gektjxzfr.sHtML


<!-- 参考信息 -->