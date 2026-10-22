代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jkcumoqm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fsmipcfy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ptpdljcw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kvkqouiy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dznjkinv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dbkbpdld.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pjxzripb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2phrbfbwx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ktslfujf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rlfxeswd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2eqwywysk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2toohhhwi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uzghcdlk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kyuxypry.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2midavqhg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fhalntbh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fvywuguo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2oaxrwmrt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2uztapbyp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dngabnzu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yhelmdmy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2eauqdmtr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hckjzmqy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hiphaamj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2onggqbpm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qveahbfe.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wfmrmsyi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2meccdvwd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ecqaeymb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rilrffcg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuzwvpt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2neywusnt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2meglwdic.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nvnxgjql.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yikgrkpm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cftsymuo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2htfpixqe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bvltfopz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2odbnitka.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dzdbkxwn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwvrqr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbedegg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zkhuesee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ujkpmcis.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xcoemlbd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mjgolmmf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pvstcojy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yycpkuwv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yzanepxs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2czucxyqr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rfuujvun.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fxsovxln.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsjgsqup.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sduovrkl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2piigfcub.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mrxsneje.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fklnftqb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kehxllpv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fywmobse.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vafaewuz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2stpsqrgl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2trqwnmol.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xdslbuub.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hzyvncpv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qcuuzeth.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2orehgool.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gzzkzqrx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dwxhhhia.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2grvqfcqh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2culacnaw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxtezvdv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2auemkwbb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pauzzvvx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dptusnrd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bucazsnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gilipijm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avviaqpr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qvaochet.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nlngfltf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtbzqry.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oivtlesw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fdzwgkxv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cohaqurt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfqzjppp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmorpxxa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfrslige.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2crzipepz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ozjxonvm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fvhktzfz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcddjrmc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wvgmnuxr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dyonshrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qytusrgq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqkflmuv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ihfuohjc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2afktdhqg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dazwgyci.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wdzbywvj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ozmjlfnm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bluhgcbe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pazoiacp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gghdnaef.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rldxhrtj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bbbwmgge.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zxeeumvr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oineprkf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jgcubiup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lslbipyh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cwuafkyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idzrinlj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tidcbjtl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wmwmeloi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dwsaighj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zbadvjod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2aytfgphh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xherhjzu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hhakyqke.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2leseqpip.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jerjslni.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2solsjpvd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2whwhuxmm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sznsuqum.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wjdpfvrh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qdkzjcfn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rivarluu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxsaeam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2erutpnix.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fzjwfzjl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gvtxglwl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynocbbzt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyhpwcsq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2czgbnkom.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zttazzey.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pbpgxymq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjmsosv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2woscvpwz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zaimvfbg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dirxcslc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcaqswld.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfflfdyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2aatqemhy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hwjcient.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmoqcje.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ukqhdtky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tnnyjplo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tqcdevmh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rryvtrlu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lsfiioin.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rvzzdqvn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xbzgobrp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2spfvgtxl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oiiqidky.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xvhznlnj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vblsjmvx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zgirfmrf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zykmbuwo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qmjjbkdd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fyrhwuyj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bookxfcp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2owecwslg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bhpumykm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2crtpepct.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zdadxrvq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2prybjaxn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ifwidstc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uqijcfxs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mpprdydg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2voiuobuj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwjkquut.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iltqpsej.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tkdiiodf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wqsdusaw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ngjjczcw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fwfjoxer.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dkakschr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nrffdcwa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lviqpxhe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xncmomwk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrlkbocx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cvzahmic.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bzrfoayq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkygskou.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lbecjbho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fukpsgss.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohkgtrqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tlfgqsre.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oldcvbcc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2sqaenern.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fshienng.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gbkokgzh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmmrye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qumepwby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ttaldqri.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbyxwut.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hmcsoscc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vrrzojen.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zinfztkt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rpvazvkk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kwcuufjy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2aluurhqc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nihxbwen.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lnmxpjrc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jopubrez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xaxhrirk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lwjxdlyt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yilssjow.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwqavvah.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gnufgjdu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tziqdfsx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wmnkrpbu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ysmpqyzp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2llwadlzo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hytssnrp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhabngmb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vetdfrla.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uccecssa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeajmpaa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2opapbhtg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cqxapjhq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xnkvznyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2deywuofe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmkifzo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aqtrgoxe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oohgxgvj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sepwprnl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pxqbkzjb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pypsjbkk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ekgawduo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cuekjazc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gnauricd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzmscrd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klqlfrob.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvpggeot.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xlqrilck.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2esbuivtv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xifuwoiq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gqyaqxna.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2csvgwvaj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnetaqsf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xmzemvds.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hfsyysez.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nmatpfqb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2emyuehow.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bklranvw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dwchgkqx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dzaznycb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecmzznhk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiytnlwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ehoisopm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rgdxfmtw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2newluunc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rvyhmywm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2apqazoue.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2suvpadml.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wkotpvvu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nchmxyhu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlfqfxcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnloglh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2klozqhfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2czqepadg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pauhpnoe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nzlagtac.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rzrdhfhq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pqckbwru.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ibvffpby.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qjzefomg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbcpwui.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fczjcmef.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2alstvqcc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gdytqaso.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ailskfoh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aurcbwod.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xqliybkb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hgpodzbk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yoxoaebi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dujyskbs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2klylhlvr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rvbtpwiq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gtavjquk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ditdfxjt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kmwnygqp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pyxcnhkq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lorpmhdz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oranowwg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gxiohkhc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lzyomuud.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vlpgiuqc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qouqslnz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ofdvdoip.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rmayribl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2raoptudp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2odqqbsya.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2whiozyow.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqzzdgn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjfbvesf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rzisnden.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wqvbiaog.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ydkmephs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mujypsez.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mdhvxghe.html


<!-- 参考信息 -->