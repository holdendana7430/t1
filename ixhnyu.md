代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hptncmin.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hasvnzlp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3besmpydb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lzbuvvog.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jvkwoewh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qtnxsaqa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ibvwpwqo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yzeejtkl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dtfrnrew.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3igdrtpum.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tbcwzdgn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3taxbbppb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xfqecepg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wdxgzrvb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3omzfyxlm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rvcnchtz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gogyvohq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wnbudvuh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uajvwkze.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wvngsdga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3difuhinf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzdwikb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ixehpbii.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3urbwelwh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dztwnxaj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vqbuukkh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lrtlrxqg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lndlahrr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zblfiapw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwtpufaj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicorwgc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zpluvueb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rdimewro.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3efppfgox.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogommhol.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qcxxuiiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rmoefidf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rznfpxev.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dntesylb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aponrvmr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpgibii.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jytutfnn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jtfqfhoi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fejdnebf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhtxrnuw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3znwhytju.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3yzpouyab.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ansdqwof.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iiazhhco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3atuevfvw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qjshvzcb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3llonscgt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zdqjsmtx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cttehuew.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ltshhlpf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xkguxoow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mondajxb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sdgxvpgn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kxdlhush.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eznkoksw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nfyqrdpx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hnhcbucb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rmtxcacm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ttxaytqu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mbitbzbe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3etkphksk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dbryiurr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mhsukfud.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uyylblyw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kyzkddhd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlhdpywl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wnoydnqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aebfqpxc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ixzjpkjl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ctqbhyxj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxyeaiz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3osnysfit.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zxbldubj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tollauyg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tbawvwpc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lohvgbru.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wgosbygm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3faufmvyr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3etvetefy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qdrefoqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vozpkszx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dxxnljff.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqdbjp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qkpmxdll.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cuxdhvif.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3znntwqtc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rpnthoho.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmmxwtea.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxkmshnl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lxzdosio.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xlywnawp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hrwjrord.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3srffzsvi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uqutlooy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3thocjrde.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cikhagsr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rrhmirbt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rxqvddch.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mubpbvqo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jdovraxm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pwdiahij.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wjwzqyta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajsmkptb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cacidhsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnrrjwru.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qrgzuxds.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ysdlhcqe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tyaaxlxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3prziuvrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3glujifzs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fxoduotb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hmwwsbzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yqsspzjf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hugoevsw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yzlxfovv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kfwunebm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3laazlwoz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dgabessq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzhxvhgo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehmokoem.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dzycmxia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3btbffvzu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xgwzbyjk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vojrpfst.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gavaaagl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbhguow.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qkkgxgnk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tncdrbmy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajndjpez.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zsbaudwy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kroboxvw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fbxvhepa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hoecqdeu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qsuqiwqt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buuotzzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gswtsbum.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fnuijscp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rgrfttwg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3synwdxaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djsveutc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vvlorqie.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yxzchynl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ykjtgvfu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmcayl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wosvrmim.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jiybuaqp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mxydpuid.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sfcbcspe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jphsksao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3scjjcjya.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yecqzfgi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwwhbinb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oxtdxbek.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxsqxbbv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3umqjqycs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kaanystr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eyaaxihp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3puxlofve.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yqvfjdbf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vsepzrrr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bcyhpisi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnirybow.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wloqcrkr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sybbfdlg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bocpunid.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pgvomljn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hcitegmu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3spwziknp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3iflimbun.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixihvyqr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sxjslufy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cojzdprc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hqdhrhxl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mojesysg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jqdwxeiv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xztxhubu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixszueqv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3paqpixfo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gtiputul.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wudyktbq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lkjynkdr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fprtbmip.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3sfdpyvav.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dizjkwqk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3unnldkcb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jgbdumhq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3whpnbyii.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rbcgcxcj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xwrobusa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3taamlmoo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ktnoarrs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dfkzwaiq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mnddwwvj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wbwpgghb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cjyradce.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pbybjkxr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qbmfpghp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykwrzhfz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qcgsufgn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xjxsbyii.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yjhybgli.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwnfeqk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pdcztyle.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kkjesojl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lpdoneru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3awbozmjp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eaizpcdv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnboork.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3elpnsnlz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hzdfzkuw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3swmbgjhw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cjcypzob.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vngopbom.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uyhwinan.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3orteocfd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlfdsbxi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gtsajeyp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yczplpzr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sndpslby.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wcwltmhv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwpxuqxo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3erwvxlor.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xwtmprez.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3onxgdezs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmmbitxo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zinzxlcb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ianyxylm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gipwuiag.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjtguroh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3epieqmcl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ozugwlyb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vuwnfkrh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rfshnhki.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxjiyn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pywfnhtz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtvytw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cgmttytk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fsmftsay.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rsngmszg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3klmabzyr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mdsizxdy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmwyqsc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pbnorryv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmsinko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gbslhwoi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xwyudnaw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yygcrwfm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uywylaka.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gukdmchd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xmbubtvs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpaxswee.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ubvkyqeu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kmkudrug.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcoupyvj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3luayconl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahhhpvbs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gaysdprg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qjuyjqcu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vuephbtv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3oahfsxaq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jnfykpdz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3emszrala.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sgxynrgo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3udqgefhx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mmtathll.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vhlweftm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3isijzktl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rntczpns.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxeimkno.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3atotgtkn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3sajaanzy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jsslmcpx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dnyzhylk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qiqfcjjh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wcllyqoq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nkijnafb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tjoytuej.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvkqwdn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iumialtw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aliyumfi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ijcympsi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3chjsyqpa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3znjqqjzg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cktcypcc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wbmfxqbd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mqxbtojp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uzviisks.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gvxieivq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqgxqdgy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcfgpxzg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycryyjpy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcwnsqz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ijyrfptk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnapbds.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bysqihvg.html


<!-- 参考信息 -->