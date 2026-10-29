代发 wailian999

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gqcpebsne.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gdghnzuuu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gboowjhee.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gbxhkoulp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpsphynsu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gavulwpau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gnjiczmug.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/ggrwmsfqq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gvywrblwv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gowyahalv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhoccpzi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gyyasaaus.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gvcwwicqm.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gjcrnwdmt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdblxtdxn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gtimceysg.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gkplbcfzg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gygfurahb.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gqueedotj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gpajpvjrc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/ghbdkqlsv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gcdxvhher.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gytvalrkl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gefzwzuey.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gfcvbvona.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/grlkiiynt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gpfjngnvh.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gzugfqkjx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtslskqai.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/goworrsaa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gbojaonsy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ggdkmhhoq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwhcoxdhe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gszbpedrb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gtnetnvke.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/ggljjobrt.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gpwcmzukj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/guxmmruhs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gwacsqnmy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gsdukqbri.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzszxwsfy.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gsejupace.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gfwtsxflu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/guotcgdzq.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvdnmxmuo.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gewkbahha.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gouqtdatp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gukewkeax.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gkxdzfknx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gnmzdatcx.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gzlptopdk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gvaqywtgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gkqbitrms.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gyhbhrnfm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gccbreuis.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gtddrudva.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gdtohgtnv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnedadfac.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gqngncemg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gglbpaygt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gmlqzzate.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gxdhxoxbh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/ggtfcrhgw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gtyxfluux.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gjuowyygl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gdeyjlmxk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/ghbytwevs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gtyzledxs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjpmjwmij.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gzloenicd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/ggsqovond.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gbhxcsxdx.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gxmstoifx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/guptsmwwn.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gobyitusz.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gzsandcfz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gbswtbspd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gooefzdfo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gmzotyaet.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/grjykykpk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gbgeaqjat.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gebsllyxj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gcanuifmf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gtizioqyq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gvrzixgja.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/ggslmrvzu.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gbmzfwbsu.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxnxxvnxe.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gnggrmuim.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gikxzgdfz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gppittbyc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gwtaufmif.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/ghaisxdhb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/glicwbrzp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gjklydfti.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/glnkcsbiz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gdvyzkcjq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gerjiwmsg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gixjzixvh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghjdfufoj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gzxnpxavg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpgjmiyzy.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gcngxmekj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gzvscnfhh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gewmvwngb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/glroeduml.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gkridbqyb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gxmpyvhrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gstuqyrxj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gkofyymnl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gkxclhpej.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gccshlvgx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gdaqevxoj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/ghqfmjhhz.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gqvamutij.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/ghwkmvbsp.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdnzegjlv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gmquwqech.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/ganptgdim.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gbojylbdy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gzopbrbzv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/grgvurcww.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gryhqqylt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gntqzpkyr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/goghaahiq.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwvatsohu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gavqvvkqb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gsepxgsvy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/glpyxgllw.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gonmnrzez.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gsnclvgpv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/guocqejdu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gingwfnfv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gvagtcfae.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gaxsseyxq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gzyseatkn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gricfnxeu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnzhjpquf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gkxqxrbcw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjdpujqtu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gknmbubdi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ghjinlckz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/ggspgdnff.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gbdqmfmmj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/guckkkoks.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gutnvnrbw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggwrznjmy.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gmtgzscyg.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqymljiqt.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggibmbuks.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ggtesgsxa.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gtxxotcpm.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwhnhtb.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsqpimvol.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gnxwlcuwb.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gwygxfygr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gtxgdygva.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gndvuzqwj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/ghldglodf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqgwllsga.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gnyszsems.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/ggplkobte.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gfbddviuc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gclykawlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gozyigcsa.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gbqpzvacc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gilvdsetc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ggskfogki.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gjlwzswnu.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gebfpqlfa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/ghvsopwrk.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/glkapljrr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gwjsfpmvn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzrgufjgh.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gdtoikymj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glfmxnymx.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guzbvszio.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/giaptinmp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gwipsuxab.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gpvkypwjk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpmybllng.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gfeiqmdlh.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gbemdyivv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gpzihrapj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gknjtwikz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnopixmih.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gajbokebb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvcpmxufq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gjtfmgnmu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gzsfxhisy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/glwnfgnzn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gfkkpclgs.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gtcclctno.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gugqyngdv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdbhqnvfw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gobiikfiy.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gvptuczfg.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gidqlxghm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gdppbnzkt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxldmmlgj.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gzxhcgcdg.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ggqxgglal.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gnrjwareh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkojnufxn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gpllpouws.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gduixgfua.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gsikhgbai.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfclbmtqc.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gfvyojrrs.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gbcejhkrg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gsnwmofst.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gwztxqqcq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gcbnqpglk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gveossnzs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/goqplpuzm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxjjfmkuf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gcgtsstnn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/grlviesvp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpqwzgije.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ghlxyjepq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/ghakmjvwh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gtoinhwmw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gfpkozaly.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsioytcjn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjevktmxo.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/ggtdwairg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmvjukcch.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/geqxxhqnf.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gddqssuob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gutkhogle.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaxnzpndr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gzyvweasz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gukxyvuvp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/ggixwvane.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gylgoygmv.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gmyyawvyy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gahpfeqyw.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gdqasagrm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geutmksil.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmpsrhruq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gswvlzchm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmjrqtrjj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gqnvovkrh.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gvpacmfpl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gksgvkrfe.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gzxebguib.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gpyyufplx.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gvesovcwm.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gejsuybnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcpgcgqgq.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gpzhbpzpm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfudllgmi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqitrmhyu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gclqywamn.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gqicphrqz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/guhqossko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/grylkbahk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gitqjxswl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gagnkszwl.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gcvihwmik.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gaxkrcyag.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/ghmpszxvb.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/goaitsger.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gepxjdkez.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gqcpsdcbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gojloucab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gdngmrvam.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gufleyxhr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gnechrazw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gdsmelgba.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gabguogkd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gpgtpyugp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gqmjqmicp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ghlzfhnin.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gjlsmddqn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdtoeimez.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gywbkdoao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gaxhxcmxw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gymkondrt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gbjbufcio.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gshnjlppf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gacqsrxer.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gthzefbuw.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/ggtngqett.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gshtawrmx.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gtofwziha.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gipmlkhye.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gmcbdtupv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjllvdihp.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gutomfbtk.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gzgtsnmwp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gvdfyabcv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gkdhqtrju.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gckaohner.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gszcydvtv.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtsnosp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gbcskgxov.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gzfcopsoy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gscuhvxti.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjebqlqaz.sHtML


<!-- 参考信息 -->