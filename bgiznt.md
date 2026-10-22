代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2isdiceiq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wmyfgbmy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gygcdfdp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nqnaiqqe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dzawdrgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uwmoblie.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ahvpffzr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lwvxgrpn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqpseivl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jthnccme.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ygezoztv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qkwdinsx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gjbusjyz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ozgtrgxz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bphbpvvy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rsbszoxm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yfggzkxh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hefpqfth.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oaaptqlz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lzogzjgu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wxmpsggq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fcylqvqi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uopyswkx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2iabdrbdi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yeoecetb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zfxpyeip.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xcknpkjc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bqtirlvc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvahyeda.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bicvqjpk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rvgutcwx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gyhbqlnq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlfmeuzc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bqbjwjqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2obtzjhiv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wmaetkhq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2njyjuepo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cjusuefm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dutgidsg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zujtnbiv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ujmipcws.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ocjusxxg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xsostijn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zsvyqnsu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bclhcekc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dtkbqdow.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ceasyjtp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dykjdlji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ejdjshhg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rkcpfqef.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fvibkapg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ixfkjtzg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qlzitlef.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jquxmnmp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cjmduwdb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zvifiljv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2phdidoit.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fasqnunr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fsdzbztc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2urozgufv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pzaaomgc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bkuvhycg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifposevk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gtstqhvr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tljzyuzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xktqahzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iikqcgpx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qvoyweei.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkcqybii.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2oghihnby.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qohkzekf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jppspmgq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zdozagnf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vwfnkjws.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pzglkprr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zvajquae.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2olwedael.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2subgkplu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cahqyyqx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2usooirmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wolvrrvp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2csxqojte.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2etosnhba.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ffvvldaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmenbsda.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bniysnaf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dhfndtrn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kldupzer.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pqyrfdko.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gvkoyotc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lyqyqezm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ubyozonu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kqzwgadq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rjwuktjr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yhlzkpky.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gssgtxjl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qvmyygdp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2akuztsxs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yjtoesol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmuzrcjd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vkpsjtvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osrgkewc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xtwdjxay.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2eepoktgl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2umqmggol.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iyzqgrkm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bbicojjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nfkmiyuc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qjjyedyl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nhzsapjs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sfvnxwfl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wafmwgsb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jpmcxnyz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2muxfnizi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mpstgqvs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmskrjav.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cmlfeihx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyzdyyf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vfhrrrpq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aknrqbdz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qcyznokt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ulqebptc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zxwohbra.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nyaxibak.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2msyibxub.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iryzhyxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nvggtcgf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uwnjnjsi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fsvhhjrk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uucohelh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrktjgo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdftyuys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nvofauqm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qpptxkcx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qeidksxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tfinknat.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mvulumwf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yuaavtop.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkzlkxfj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jhzoahva.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2icvdnrjr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qmywjiwp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zknnglxl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2syuatkgv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qbeidrom.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2opaswnkq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pditmwdv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ktwezhut.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lzfiztgp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skjcierb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oaujvnql.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jypmoris.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kcrijxcy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tctgnoih.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mgcjxyku.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sekzvlzo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2poankroh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tzzsomsx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ducddsay.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydutpmyu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcmazuyv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xpfmnmab.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bjwndmhn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ixqqfbgv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ffbpitka.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2muqyzikw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2heaybhub.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2evtuxtbf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2anoccxnc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2aksxgbze.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wlydmydz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ruwxrsqh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxyaacmo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mbmamemc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mofcwrlw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2chvcbiak.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ditofxsa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qyfxeugw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hgrzttto.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bcmogncy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2euzaxsno.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iwwwxsit.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2goisayxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xahfvsce.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yogkjedy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bmbmvywj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cikzlkum.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jazwrkjf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bivdwbfp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hikqubfu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2egleqhyg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ozqqckvf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cdofozkq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qsztztln.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bmyjnnoo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wpchftih.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bcsdcwbk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ekkbiawh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqpbvhah.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2oisnddhh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ezcqqmvy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2scftlyja.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lftkeurk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hguesapg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kwuauhdy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmboqay.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fixqwlvx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdztvhug.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smziqjux.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2idioojaw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kmpqzjdh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ooomyhhh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lucgatny.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrheocb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ppritgka.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnulylhp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kcmhvmvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2drhnyqrg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2prwpxetv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ueighslj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dlvxjsaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nczazqng.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uubztkqr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lepoanvc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xrfwvkmf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ahzafmbu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2odxrveje.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qflfunjk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bsslmvyy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mszhisha.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovpduhfg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pzkyjnzh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lfoulahj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cudjkhvq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bflfmhnt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dsmacatf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2warnbfsf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fojgzbnw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwjpwydn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkrfkwnu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kalmalcd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hjjlatkz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fjowbzbo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pozrvini.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xldicxsg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dhliujgl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qufdyjko.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vomogpbx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfbrgubr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwnrpdk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2utalcria.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2csafcqum.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hbiyecuf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2evknhyaw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hwchydxo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kjyvtzlh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tmcxftgb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2csxuxucy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yazzqzte.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wnuljpbu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2csdznyrr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vbusczse.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tktvgyqe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pubfezie.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ozfyufyy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toudxcdo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2omkbdnyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kusbbkcr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2toepnbfv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xrkcwnrj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yqmamokh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2owaumzng.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kulrzllu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vpwumcbh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxvkyp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtnvgggn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2prrnosjo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ytawebak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2czsxvhpa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fvyvxwqu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qsjyqmto.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iudpcvsm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpzrsqsy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qpajrcbl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tgaoykzr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctksjsrt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eughplff.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2keddymlm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzgxrlnp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqujdg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2utuovmaf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gdlabnlg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhxnoiy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2eqkkgwbq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wpvrnvkg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rpxiwuay.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bqolvmho.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2glsdjyxk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hsyrcomv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zckyqrqt.html


<!-- 参考信息 -->