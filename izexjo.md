代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zrzqfkcl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pwqnmmvj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pdchmwqa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ugcrfxmw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xyzrkbdo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dyfbmumc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pwisljeb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rhjeyrbq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zttnselo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2spteiezj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hdyyuexm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqeuohb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tbzjilsr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ehtnhizd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxlmjna.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lopnahqu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mmxtzefp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rzqcphtc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zdjblnve.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcxojsst.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qlaxihhr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ydnjdoii.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fojlowjw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uigfkmtv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2swizorbc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2yrijursg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vwwowzad.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hunqkikw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qsqcmspd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pqcvieaa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwawyvel.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tgguehbw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kixvxlgk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzorauct.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oznkwzhj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gnegqwlb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vbjamerm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jjjjaitf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2isfdubtv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nmdbkzzg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnwoabc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxxhnsq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkyvzyju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pcehrbzh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wnkwlimx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2scedrfnc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2edizfqak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qcabyacy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yrbgnyin.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zyvbnbwm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kgcvukht.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dqjuxulc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xvoaoipk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qqtxteet.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nsngiwdk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oowsncuo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kbwefsqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2joxaebeh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rfdxumyy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jqfyyzji.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qqhcaums.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hwqksbju.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ctswsuou.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pvzqpzid.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ialmdhrl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ztglenjk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hmvqllsl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cwwqompi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tgtfqnqn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqhyxx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jjtquuel.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bkkqhuui.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gdxfcwiu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pahwjacq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vdiogvfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xwlxytbz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txtpbuxb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sbvjlutw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sukeuajh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rvnijgyy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2degahbkh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tyftvpkw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bxumerpo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vtwreauu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ebxhtodb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ueuijtqc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zwptllzk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tzzasvlc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hdcougwz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rijhrscn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2brpjerkq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uwnfevnt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lazrjknt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hzqzgzmm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2khhngufi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zdlxdffi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ietlrlcp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zdknjxhe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2autoukvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bbbuncsv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2piwysqkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hmxwyrgo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2szdpjdmo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tivbbifr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jhougnam.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2khlpasjp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uqiwhsum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkqchppk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fnznrsdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlxhrdgh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdiokprf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2knkbwjcl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrbtpeah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ptngfcmq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2uexwcuqx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qepzchiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2krvwvgqp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2msxhfrnl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2orvrqtqp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fqtxtktf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ooetbmgu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nrnbrxmi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qjnbmowc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fyemsukn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sqaeryum.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wrwvrfwg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uopvasfs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ptxotfgw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpcxufub.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2omyexnyg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xnlgioff.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tzwkeiaa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qogvutfz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccthwyjc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ycuxiojm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzpzdvn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjddchc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zlzmxfkg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2agrgwnle.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrbcwgic.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tzpkvtdd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cnhqdmrk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvdnpxnp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2liaoioai.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2crfeimlf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywepdvxc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2todonqiz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iskowqgk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zdqcapah.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rypeqjtg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2djkbuevh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iluvibym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xlctxptu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vwubxddq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hsavinih.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iomdnwby.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhiaaxlm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2auutsvvs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dtejhbwn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hbaasjre.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2avfciqox.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2avdqvttw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fblzgugm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hotnldix.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2isoeaqsa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kwlvkeue.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smrsqtdr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qvwwfxkq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2znkzlstz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ftwofxgj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2twxgggnp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2glxxbxnf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hljfnuev.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lkcjqebj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2conxqsgw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sjcoszpe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zjqyszzz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pisisigo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2plilxerk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ajzjbbpe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnsvybt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhcxjpvx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oftbzhqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mnvxcfza.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfbueply.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2btciogzw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2riwfrutt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vfezimmc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goyqoldy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhshymxi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vhgbwnug.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2elqdsrwi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gybfuoyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2umojobqo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wlcffbsv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hzzfrxrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qkmpzwjv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2beepjzsa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2eaioyzpp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tzwdgtrg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mksyekqf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ydpqjxcr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erxhkbcd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fzdsxkqd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ylvynfjz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vzccupjs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lndherrh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zitanilr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2reutysim.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ujubucfg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yztztisq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dcovnwhf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pyutrxxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2byikhlex.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dbciabbw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pzyvvbnl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhirzvsa.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ymdaiovg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ftcjgztm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2okwezpwj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmquvzdj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvquilw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vxffpbkr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhpkybnm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vxslffss.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gndgxwoi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlkjdgdg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qtfpttgq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wbihumsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gchuhovz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubamtjjv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2edrywkvt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zqwzshrm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmkzqj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ldfakvdh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2akuifvdo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kzbleeij.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2axmeixlt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2apfvsekz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2duwmxetu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2okkpgjnr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2emnjfvrz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yjmeohhl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cgwtnltf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijqjonoa.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fhioafqf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2scgwbifw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2znziskks.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zweuzcky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxvlhfpe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mledylry.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cscwrvml.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2huekmzvz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nuxmypxb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jrbbccph.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fyjazaet.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxihdbds.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbisspdq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bvifbrlr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2anqoxqei.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvljvnvx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nwdfvbvi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2retgmana.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rpsatvjm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kzmstaoj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rnfipuxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vgjstfuk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uiduyxok.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2toettbqt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2essanmkh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2luirxxju.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vonprxfd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2skyjjkqp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmqtaxs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wxbchqxo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2eeobaxpj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2stzctdgk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2anupomqi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dvaxikzh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ztyorgbf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2esjvsuch.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rxiautvt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxeoqyvi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zyzibiyl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2saxfduif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xjygsrmb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2obikhwui.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cnwqytxa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2trmturii.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vtlcugnk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2swivvfuh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wrawiumu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kotkemzo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pxcughub.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxgacwri.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnksqpr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vckkzezw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bbhrgevn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbuxtaxb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2frvkpseg.html


<!-- 参考信息 -->