代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2grxtvzzz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zvyzhdnr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rpvuqwko.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zllxzxkt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cpjmgybx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sukcklvx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fzcqvcfp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yvpxnvbv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2avysfdsq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oysmldba.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpqytzy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vtudoqvn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zsikewcp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hdbmphev.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ildxaqgc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lgjxckbw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nfpblvuj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fuxusexy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ztstyxwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2efhcdroe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mrciqyak.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dhpshqxv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ettgobfx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fvrswcdy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fbkvjato.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qnveodxn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xfqljnnv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2eznthalq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yopnrshm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qtkbpcze.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ujsbjxup.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rcaqzhni.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zolprsbi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zoajgbpj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntzxqeun.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2fesuilmy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bntggycf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvcluyik.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lxakviwq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lirjwmkl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tcndrtqb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wypdqqme.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mkaadstv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jmefalfd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nccluejn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jvtidlps.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pfsugjma.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mkbdxwcp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gvvhaxbe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hznxanaz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2usbwopza.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ybsulxzg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtcgfkul.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ytendkwx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hcvahhqw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vaocoygk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kxuxmgsl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ytuclcco.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2avtfmbni.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nygcxkfn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cgynipzq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vllvofop.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tdvewpap.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vymszlog.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gvbrlyto.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2melsbrwo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rbylpnsg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fuvtqszv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kubmtfjh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bdixxuzb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgoakxpi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yfocecoi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vczptuty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpptwhic.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zeqknwui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2byzabepz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khhvhoay.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2irxtgsrh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2laybtfzc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qknyqyxs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gidayuav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2snnadfsj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbceozll.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hxiwkksp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wooiyasg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cositiqx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwfrhln.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mszkqbpw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2guuqfueg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wcuzybcb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2drxhjcyl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2syxudixp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jecbqntf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axbkroqe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kzrcmhsi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vcqkmrwx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2omkyiqqw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wrdkhmzg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vfphgutn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2awyeriee.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vdlofwce.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tyhydbza.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ewugxmor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mjkgrnwq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wdwwbcym.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2phbltdjl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2poqhlzxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxfgnpoa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ldlyhjzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icrusvjo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ayyjasjh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jkgzbgnp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wlycectv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ezujyrta.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nndpeevi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dzpqafui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ffyiuzgi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2euittveo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xiaxecdk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2sipjxaer.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mnybumjx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mshvvtab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iafeebed.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dzmhiztq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xwhsjrjc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzoobjbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2htdtuzwk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkehydr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xbrwgtai.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgscuru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wopoywvr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rfvyjcmc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fucikwac.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2twwtuimr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2abjilpmx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ytryjfnr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sqpiabfq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mgpomnej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqbghbp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rycbqewt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2frvnegvl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2opwriqbo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ujnckcmx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2weyxnjcc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdvqpxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvqbeo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywuzntaj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qktjsalb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2svahsunb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2whxnqlzq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ujkkzbxm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wuguasey.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2puaorpog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wlzijmch.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sthkhqfb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dqvronmr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2elwniwew.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2byjoyzto.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ugiqgkve.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zchxdneg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zvtkcopp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2davrylbc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tmznfvpp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2katsbulm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bstdfryz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ehvrzkld.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dxwqlmmj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bnzoyflu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2exptmsfm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfbzejss.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kkzmkzna.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uhitohzo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rcmraqgv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2oaahmopt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhkgsnfq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oghgwlxh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ybbzavmg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cghuwtab.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jrlntzva.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2huoacmeh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dxypkslg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwtgajyx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gqaotmll.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yyuximay.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2typocmbq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2scxqgogn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xbxfyizb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2czqdaqdi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otpfwhje.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vonkujml.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ouvfuual.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rtiiicja.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yiszeoif.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2knlsgzuj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tifcqimp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dcwjiitj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lrvlkare.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sdqnrmap.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2nxoprhjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bsxbcykt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ivjfkhsg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vhtqbqgs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zznohxty.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhcpiuj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ikbtgtuu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2koqsqfup.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfleivz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kdrumkto.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2anlbpbmw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2aczxibqk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2itzniqha.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqvlefkd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2khuulvya.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zlzaqdoa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zvvtzkox.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ubnczvio.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mavjbzrc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tbgixehh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qqogsowd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2okeedonr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dbgjrnga.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdkpwgf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rqxexwbl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kmpyznfj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2uovvslji.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2boynkvre.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tjjoovwo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bqcfyrgu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kruotnsh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hpkqjhir.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekgrblbk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfcpuvon.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrdkqr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kewobqvm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2afzxduls.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghzgkguw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uuhtmtst.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fwyxrwme.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obumvhnw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dvyrygpq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hbtaxnhg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ttbleixr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bkyqpsbp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xgzrqvhg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ppecjzyg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2iytyrjnx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtxtthym.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbnosqbt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axmewtdk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nevawoyf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wobmqzpp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eawibprw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jhqblwmn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2urmsrqmo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wjjnmvco.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jafhbqwx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itmtsfto.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usefnbqc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrcxjil.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ojfneqzh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqgfpvwk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ooxvoxzs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2egfspszp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2twlpsofo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gfuiqfvu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ziuljdsz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqipwyj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2imtaagtz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2obfiixag.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2syperhab.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hdcljfrk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdpcrxrx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cgvgxqhd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpdefke.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vpeceizh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xlaetfqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhfjzwk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cstebpqw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yjqjazvs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vvjmmggl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lsexgxqb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hkdhaofl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2exbjbfax.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvpmmsda.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ivfpdxnr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qmvrtnku.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cwiahnqp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cysybfro.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2temzyfzn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wbxewwyy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cowcjdsh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rmousjjo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hmflzgmz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tborpezv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbyngmt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fklvxpbi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dhercybp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hyttzdmj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hbaupewh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xpyvbixu.html


<!-- 参考信息 -->