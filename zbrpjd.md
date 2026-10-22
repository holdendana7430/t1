代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rgagoqar.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkpxtutj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2witgxoef.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bwyynfjr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gbeefywy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kyedsumj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfcfxzsn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ntyzelgn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tlkhnscl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ifqvgapn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rkdkauyy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ouyqifcs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2icdvfahv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2guqoyymp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yjntmooj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bbgcfigl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wvdvbztg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hjktoeoc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2eqeplyki.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnnazqn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ksxogdbo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gbndjofa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yxmsounn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nznbzvlf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2amoarwwh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yodcddar.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mpypkctb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eegyaqyi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2avyvjvpu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vzpyncix.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbsbtnaj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vdkwaofv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnpvvil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2yacqxmjv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bqskxutr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kyavecjk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffgbfqep.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mvjimugt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iqbrbiet.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jgeevuwl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2itwapknc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2augjinhh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2poetsben.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kapszuiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwtszgsl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qukuxueg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rvufbrfq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cgtwunha.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgcermpd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xyylirvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqmkvbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtfkbifc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eavjurky.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sjskrsei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fcruqpii.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hsrckqjc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jkrvyhnt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fmumgbvg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqgcxksp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2temeyoqo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qmsenfse.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ivbwyrpl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ymfdqgqb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cuopjtpv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bjpptsma.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kauepnuf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fxpolnhd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2glagucda.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tnqqbgky.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oknghwel.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2foomcacw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qdysdhlq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vdslqong.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ugphgehb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2agliekof.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jqfqofnp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2groqdqfa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lxcatynm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ctwiuglw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hequryyr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nlwfxwzm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ikadkbsb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fowqejii.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltnwbsxj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbopnvqy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wzittheq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zuzbfzzs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gtpepwwo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2atrlkxmt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hpumnahz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jhjcyhdk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fbneehln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qnzfrnml.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rlalqoov.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ottdohnv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xddimvvh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ctaokzoc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cehaoyvy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dvfqwuwq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2urjptubm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coxswukm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ixuovtep.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ofsogclc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2epmpdlpn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mrnpbohu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dsqbqmta.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vzlgdlsy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yvwqtslz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aggnjpzn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cgnnrpfv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2exdgkfcy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clidcegf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gfyhjgbc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lyuivuel.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cwcfopll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txhjshhl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2seurcilp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olmwvdmj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rqwhkwde.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zdauckni.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qharqqbi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rhtxmpkd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2afnyzhms.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jkocwstj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tivjzhhc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bfjldngq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2igyqvioc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2izcxipym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tsndmolx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xdlvrqet.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wwolokaj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fegdysul.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ibslscvd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ukwtpkuz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vpxmqhal.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybroreni.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qvcubwiu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhvzjsb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cragjqwa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2izktzecg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wjeynqjs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ssospolz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oaayevej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lvxhzxid.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jsgmzkex.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xyfyfuxl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vhhwypbl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwgqvura.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dgotsvei.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bciyghtj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ovirgeuz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcblbjq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxoxqevx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rukbehow.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2itledqgu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pihedcuy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2riacglyn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yqxwnfcn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzdgyuyn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvdwaeg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2awitzzze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iiywqssk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2msoyseap.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ythepnfd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgqclux.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxitpxv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ukmzcfwv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hjbdhazk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zddqeazg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjgiyfyr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hreduzad.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ezoqfxvm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2joikdxdb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2heordfcz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjcezqpf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rxpwmzsz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbmembqg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dourxnrr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tsqpozem.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lgtqsdlz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ogbeeern.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmscvmya.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjkhkmxt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bftpyhpn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ovjrdrsl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hdmricwt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgwxpc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2krgxdjso.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2smftujoi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ealjofro.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gekgyidy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ypnskols.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snztketu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lgsqvoda.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kbplxnpq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mihhqzjl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2btmlwuya.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xrcqvdur.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2inueteem.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gdnqcaxz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2stxrpfiw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jvqbxzwc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yvonpatv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ifywqfmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2stxrfaop.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ogrwbitu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwvtpit.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2orqzpuke.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2etmsrepb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2islioyau.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcxgaypz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pyjmqdvu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2shhcedkn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2msfabulq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2navbdknc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jjkpqajr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dbhiuefb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hfhuwuag.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dzfpedjk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rgbwxjbi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbofbtlr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vgotwped.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ifkcftdr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmyigvmo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbeovuga.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjxsnvm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zjqrxaxw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2whptgtxk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ayafzioy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcoodzy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2stgycvyv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nxkrwwwk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nafydqxb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cybumtbu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpmeymbq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hgjwlrkd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lniejhjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uzrbsqhz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ozwmbnod.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ykhbpjno.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kdribhas.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xtwpciwv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wbsxxxtm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2buymynim.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jyzmtzuo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mabjnnhz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cjoputba.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ligkxdsd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uaaegrmk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ptoccrke.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uxqnbiww.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zpqpyjrs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2okmfpvxq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jhgsdvqi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tigysato.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuqdtkcv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ldadzffq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oddlphge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2whtbbgmb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rbvktxpb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2oygweprh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2srupxmqt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aacujuuv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqjhhtp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzpyhsfj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bnsfstcg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjjgnj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnfndfp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilkjagib.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rgugcojg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ozbjxxtk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hupnshjw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yzyrffbg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xmghakgj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yuhfuzcg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xlxxmimz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgimmjgp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lxmwoulb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nzuxlvci.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mxnuvzmn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ifmvwwqj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcgqtjn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jzkdqwzd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sjksdbqf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxvsqzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wnbfttnm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rjxajfko.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ucfzxuza.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yalpoekd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ultxgjhc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpykyxp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmbjvfkt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wwqeolgl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ohqmhxyv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fuerhgwk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xxhbkbso.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rencybsd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kszgbugy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gfedbyyl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ciozsodu.html


<!-- 参考信息 -->