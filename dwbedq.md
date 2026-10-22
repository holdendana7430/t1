代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pmlelcvj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkdsigfs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2urneijpe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tpbwkfsg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xllsbjag.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tpdujrgx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ejfuddob.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jmyvvmrr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jxphqojb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kgfcdguc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lzfjfnal.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kzydvftm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2moxinsch.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iovkgspt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wpmgjuop.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2piogbosh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2duviqfal.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zqhvcirx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ovcijxds.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vhidfgiu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nkslauft.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kmtaqjvx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qetvtxhv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vagzytud.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bishanjt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2elfrnkcw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kzpmetpm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fedhfhwq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2irwximgp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2amhitfvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehyybkyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fgzclzxg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ccapyckp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2prhhvpav.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dgghintb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qzkvbuol.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyllynwp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyishgto.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjkemhdg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cpjnvlmt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gekioygf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hylehzqv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bvfstcab.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hwpzxlng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2czprlrip.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2maufvcht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tdjkzfnk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mvehhyye.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuvfbvgp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2flvmoqdr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfshvqzg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2orenkzjl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iitinxqk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ecwhgxyg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ehusmoxc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbmzsxwz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zckztfzw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cepyvxpa.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzlcerfy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gtxmjvgb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mlqanprb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2octntttl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zsvqjpjq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2npgtzoqj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wwxujzsm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ohwoutcw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2newizway.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wieqdyqn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sxaseeyv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lhcrlgjr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2svyqctzy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ggovbqci.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zcgadcvn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rnbxicux.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jguaajhq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pebcqstc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2skucjjks.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ljauqrlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vudxfzff.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2voodfmpc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ppesfwks.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbnjajld.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2erjpqbdr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2myfpekgn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2komjtwyl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kkdxsbnj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hvewmklk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uedgbmsp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jkthzggd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yzrgzaxm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lcocfdds.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rvkgtwyu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyfiauqu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cfsgtyre.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgzjsav.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2osnosaev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gefvgxeb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2alqifcio.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2oeeqrhwn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2inyqzdpb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjtlwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcfqicuv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mxcuozsm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zmbfzbmb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kubbbbtq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2msghapij.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2espriabj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wgsoqrsd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fzqapfjx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bbwxtwtp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bdztamyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vjjtgpoj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rpvprmqk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kycrpiec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etzkfitr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhhlzesc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2syupyhfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idcbdocx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vuebkqsu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ztjhclco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gpkgwskb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wdppygph.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fccvimjb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xfwaudiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lvsstrew.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bzowjklu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2axdhquuc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jyumvxdw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jzptzrqn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xenexpbr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lujrxckj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kahjvogu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2phgbvnzo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqhtffb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nvrnsvlu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dgypcmdc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kbtczjze.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tttvsppw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pftzmasc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vomlghwv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwxamtwy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tbkeactb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ccoexzay.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hdswalro.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zhyupdlv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rzpwuguv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ourkhsfv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bygxifud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ghujduph.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jxrshvoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ybadbirl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ifynnboe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2luodpogd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2txvhwtfr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjdisxsq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zdpctbjy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qgqfeejh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fvtismbb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dmosbpac.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dwkfazai.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hnxwkcdj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nydshfwo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vxxlponx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ysfoqxfn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2awuindrb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2noypdxgb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ffmdbylb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yzsjwpki.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yshwytjr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipswkgui.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mxovafci.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rrolltml.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dqjjwkxu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ameikarc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dltbikoi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yhdgnkiz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2spnuqgyk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qosmaxzw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cazghjgw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wzlvavyo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oaxhxycg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kasxknbl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vtrbohyl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zrzbkidg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cwnyuxlh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zvkcghzy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lthmyzqk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xeamripk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rovdrjzv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eykoiyti.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rbcfpcwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xjxcwgzf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uhhglqmd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wedlknmt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hrmfxgxo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aqrpjlmy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhyqyudx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ivnstnnd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nghsduhr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2olffkwqw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2agulfuyx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mvvpmxov.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ovkwnhnp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2orlvxump.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2trupykla.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xekalvba.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2crechwna.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kwoheqse.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rgqjxywv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2srhborpb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mplazsoc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uymgvwgc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vkalyczb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zwmidwiw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ciuvssoz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jndoxyhk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aghkunmf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uswoayfm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gudsmnda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uegvcrov.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejnzolau.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lyeazltg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tghjvpvg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gccihycf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwfujtn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2owokdkuh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2uqcvovkx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tlziiotn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwyoyxhq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdewqxq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pxditiyd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2prhwznoj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yllolysx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vyiijdim.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sgfvycsg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qxclfved.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2caadqxst.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bfngwahm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ifkszhhw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2unkeryfc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwyfrkeh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmzdppux.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2czdhuryy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2akdmkrer.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ywmdpwef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wbromuoi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vgfexvox.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nuvbqwqk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jtvbhdnd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kkgyzkfs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cskraldj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hhhffqoq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkedtsqi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yahxrutf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cihaisbb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kotisdov.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tqcurggn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdsszmx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ftasfzfb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2eibzrrbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bmdedaib.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oygshpdz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ssbohpju.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhdpcct.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfigopsq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iddcytpi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtegfrid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2irngdbxu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2homkifre.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dvngmiao.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cwmdqpiu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rwewufbo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rlkwvmve.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xrdypwnl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fulschpu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dwrczupc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kkthuwdf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2thyiwpvl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ymonaxrt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gtoqgccf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2srpnixnq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jugrvkjn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2snqtkmwb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rfhprdhz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ufwtzjzq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tnurcayz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gkzmmeru.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kagfupro.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hltrzinc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2btklqtyh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zedorfmh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2embynpuc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eqvkaary.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fkfnslap.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pkcopvtk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fbixavfe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wdyftdus.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2giqkuout.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrwgpeaf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rndhxiaq.html


<!-- 参考信息 -->