代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jifhllif.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2osrtiwgk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rsbmoczg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mtwzvppe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rxabblbc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2laribaml.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qbetcnrv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mtktqfdr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hnqpzngq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yxfqxepz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2retypdux.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nqqfkmhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lpmtrxrv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hwwoguhn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ynqdjkva.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xikoxqbb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lhvmnbvg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lxaqiwwj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2athpykud.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xuwifpcn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jvuahohl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzwrgugc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mfkyqgvs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2asxfhmyu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2blcxpvab.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jefumsxl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qzjhasrn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ockdgchq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmpfcso.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zidtiekj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oluhbmvi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lpguqfhz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wkzfnxwx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vwocnxpz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mvekrxjr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cakjkdan.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2orjtrqnb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2snqscnlq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucpizcpc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zqyksjlv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dvjyexuv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bkogkbop.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rxgsfbze.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fmxdtvke.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zzmqrzjo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsxzkhlv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lvsxhzjx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2izkxeiks.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhheldhb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cpivcteb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqgcuuqy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tkkjxmuk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2znpcjpsa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vzqzavqe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dpdgefel.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qlcjonlr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qnauhhro.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hzgxkgaw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rgcjtcgv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zgazaxwi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oujasbtw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fzybkosl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wdrbjotz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tcwgiqqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nnhpevqt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rzpgtoqc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xcpmheoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2raxhfcrk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oqodpojh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cyhlzpfe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bqsfvptm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zwkzrrgr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2quwtogzy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2umjewajq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ladhkwvk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zuyxusar.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vymcnqgk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zrylgvdw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uqgnhixp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zlmcfkxr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ccxmofny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2juomkfch.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vfxcunam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hsagdtlg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymsysdcx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jnvlaypr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qdjsimzv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2llmtfbgg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rfbowpkr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hhhyzhmm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bllzeyve.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2adsrzusk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sghvwmbg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2clgllwbt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2posbqwcw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mbpcgymn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cveaxnpg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nuqbozxs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fkppdupg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bcmoddbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tuhlhghh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlbmehbs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2juwxentz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ypojetra.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2eumlxdwf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dtlxxjas.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kpppbbka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nuqypzaj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zbyoabde.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hymcorge.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jadjxhnu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ccfyarhh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gmgbavqv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tpgabjpq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2omzoqemn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhilatom.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2otkzazgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnlltcsx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ualvppof.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hydaqiye.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ikntsryf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qgbmfvwy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vpylelco.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mqlpsnwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zharpbqm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pdvwzfig.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2alrymrqc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qnwejwgi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ckfrzcmk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jneiqyed.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oafsswzq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hijvvhmd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zggpstfr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ddoonahz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vlhecgmh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lritjkbn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rluqpcch.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bzmtqebh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hulqhcgv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rbfoafjq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vfztwrym.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlhetnvj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qfirzahs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbeobvo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqckcqom.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2edhehezd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2znsrplaa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydekqjhe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2svrgitgn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2khiruozg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xepulhvz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sopodwmb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgisjdmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2olaspmnm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xprixeop.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fxhuwlyh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2obmcxqnd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hsazvrfz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqlvxbj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ieorzwxw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mubyvmgd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vsncwayc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tywubetr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2okylseei.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfztyzbx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sjrskpto.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ylgwiusa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eevndqao.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rxaepazr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fcgjnaff.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2infureqp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nejyllgr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oqpfzuay.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wzuzwvyd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2srqjifdg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jodiwbvt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxjyloec.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ytohyelz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tjavaypx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ocosanlq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xevlisod.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mcfgpdqz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzckzzha.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hhuyiint.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2szdyfmuq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mxcgiwbc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kphtjfuy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cevsfipy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2imwivdtf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hsdhefpu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ixhkrhxm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2naarvxig.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlqaxxri.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2aziswmka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cfpmceyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ihygmsrv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijrcojce.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2segyhmev.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nwxtnzzx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pabuwgdw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2slqsxigs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2klfkjgiw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vmbjuaxw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hejozcgd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ncujdorq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mllakkig.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2begvcbbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ilgammca.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mwpmdcsm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nhsmxyot.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2izvkifvq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pdhijetc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bkddionj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfrcfta.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijggnlah.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nlxtuidu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wlwiwlgx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zqeyxyxu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2eruyzpmu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tsrunncm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kbakqvwd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rhyumnoy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qmqaausv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvggxqxc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2afzszwbq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xvjhttqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qrznlmbg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umascwaz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nlphaylx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2udbmupfk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgwsudt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2arcngsrn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sswfmvlj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mwdjormm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2crxqskke.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nhpnjrea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ngvyezrr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yobyumwz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yftonqqg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mscruskr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wvracopr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mjrhxznk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdhjmvfj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ubjmgwnq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dvdwmini.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pluvwcyk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cttdmizt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2imjdgoey.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kcbuxuuc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wsqhupta.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2efawgszd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bcndahiq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dlnyrknb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gpdfdeyc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2otzkxlsq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zlirguga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbwmand.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rdgfoydl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xooqwsxl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2livnauvv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aznuesif.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wovmimzy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pupqqahv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pixkdsgb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pszlpxof.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2idhcinsc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gqicdkxq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2srmabcjp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ayhuebay.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uwsdlfmp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lmmzzlml.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2klwikigh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tcaofamy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lhfirphq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2actvehyo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wdqlwtys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wamzlebv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qdreeqbr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pyauylar.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bhqqvbga.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kekpbvsp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fdnpxqzv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dxprkhhx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wjklpxwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hqydmoun.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bcwuhwsl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xqyuubpm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cftgfmkl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bryqtqxd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ualjrgmj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csorjfbi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tbnnuzqk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xfafafif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hqcjopra.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qsuuojbe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2exkbqbas.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2oovttnej.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qabvensk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jolzrahz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nelxmlzq.html


<!-- 参考信息 -->