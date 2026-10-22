代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2osiorpdw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwjqtzc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vscxpdck.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2swnkqfdq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qhkhofxz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lpxefakb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2epdxtrqo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kaitktfc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ykkosxwg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oqiodqas.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zftcfmyg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jmuwjoqp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xxjthlxf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rcurdwnw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2twnxctli.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ribaupht.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lecjujdo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pvejfsle.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfwlbjr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aacbuxnd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bggdqxbp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qasqfeod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2grmiprig.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snaurzoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fmmolgqn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2avctugdz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ewvuhftk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jmhetgnb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2oyufzfgy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ueafnhiv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2voedkjsi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vcmywpvu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nbglmyja.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqdalggv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2umbrghjj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gnrfticj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2atucdiav.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjvirpae.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ykyeamfb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2anykouor.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2agjibkkn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2exuryjye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lxjwkaza.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2psfayxow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2caivlwuw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfwairxf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgllsvma.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2awmerczg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ponsncpf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kufqxmfo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cptoqdbj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lptomgdd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fnhkisga.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pvqwafmz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tyqwpocc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mchjyjaj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lewfkrko.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cfwlvjhb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ktdrbnfb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2avayfwmb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lxzckxqi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mibsicxv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kceidlak.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cnuugamm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fxmulhkx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hqbvcnba.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dixtpgmn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ehakaond.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qkkzocgv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oxeoybys.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wfxwiyvi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnaxft.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qvaxkgon.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zbqrhyfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgoslxwd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2olhemjim.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nuzqfpoh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2agjozrmt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iflokfre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqfjygru.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rhpltbat.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hitgdacc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gecinwyb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2phmtmpcg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhwdeicg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cjglnahd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lcyvzogu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tbxvawru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxpmrii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tvtnitpu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2oslqklwi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2clxvuujs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2opeqlrtr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bvsimiza.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ozfausnc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hjyeobam.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ngezsxyh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxjyohts.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2amcddkof.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2anqhodci.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kwdxlizp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fthnbbbp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2obaqgplr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dtcswmzv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2oxpkolcc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pihxqpbo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jsbcfymn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvktvcpm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2izrmbbjp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xboxymtm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bcxrsaez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiftitlb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2iuiiykuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yffezisq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2scinpvwi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eqlpqtwu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2erqcoeyb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2emlfkhai.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2svmivfla.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wsawruoc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wmrwsejf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cpsfkgqk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ircckrvb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jglldfqz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yvtncneg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2goykbpsv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fhdbmzuu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmgimjyu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vinzvxgu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wltfoaxr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2naedmbjq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nikoylle.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sycsxgmf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2aghnwvhg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lepwbbum.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2flkaoivk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qmllwemb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrngxcok.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ilkloont.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2urhjxtwt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlgkglgj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bbifiarx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2skaxtwla.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hbwheinm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sgmwksic.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ehyvtzrk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wkkdatdp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ebawwgvb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qaztcjad.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2skcsbswi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xvyxpnvn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jbnucztd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2emghqhzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wyvclmwk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hyhtvtzv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bbgvprcs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2umijslvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yujndwnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2znvgnyjb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2swbuynir.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glsjdejx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nuhagkir.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fasjquav.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ofxcfsaz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2feejbwre.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqbvufak.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jwjjpstl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cxvrwjlx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2msbtzilc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zpulglgb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xptrwpnt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ryqgfhmd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nhefcsae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxwiiwne.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xpkibyyf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dlwywgeo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfxvtkdo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lzkwmpvf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvjspnt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ptycxgkl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lyeguzvi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2osetpevb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fshclxee.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnqklhl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmluzfaz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kiehiddg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ecpxglnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ekiljjrh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjaabyf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nroxialn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rhupfwbr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pxwegyar.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjaqjkw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cyavhxfs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bbljwwvf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2whhtipur.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfiakih.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2heapvtoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kntthdgg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jhwphjsz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2klkbjfes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2frnjgluu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pozmwixe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dnmfwosf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvevyils.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yiwdioxz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gnwsirqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2klxlvkna.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ykcqrkbu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tudwwphg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqjmygkb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iweovpzu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bpaokcup.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2knlxlmih.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwkkbc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hkcmxuxf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sfytnifh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vkmogozf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dnlzqspu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfylmkpy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgeqtycc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2taprnsuv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lbjbirue.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lxkdbcoq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgziwwt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzquopf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgaoxee.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xvotalkl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vbnoxucp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmqickk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lvicvykq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hkxvgsaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ziflfzmw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2scblieuw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kktqpqeo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2owgodmpj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2krqsodbg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwbuxagh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmhgxbwc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eqtuuysr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kovagahs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ypdkukkg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmsvadzv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jzwbozgd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vlnwkbgg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hykgbikv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hvpkgkih.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2crricnob.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2upzchcfv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2buusmlqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gyrpnutu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrxwrclk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrzhnavr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hocqanke.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oicsiwoy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nyrckcci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bfzcyjqi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ydjgoawm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yeehhenm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbchojax.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwteotfn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bmqmexwr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zekgamls.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtjnrgml.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccgmeqaa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ycdnoizs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gqaitewz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wlacdwdh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tpgdpczj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2swbuxuoy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kvmmdjag.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xcduyaly.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mpgcatfd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yforyavo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eepptjhp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jgtchvhw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nmkzpdmi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bxifpzra.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2apgoxqhy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zfjwrbqf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zhrvqxff.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fcliicxw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rwtthoek.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hjgwvdqd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lxhxmlqr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xfocfodn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ianzlfzx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyosucwl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2khdzutiy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nvrrunwa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dwprmqwn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pcqfswwr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eqcgfjpo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fznumzwi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pikqlrja.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gyutpvlg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wcvwdevv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2itrfkhgr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2risswnel.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duodtxvr.html


<!-- 参考信息 -->