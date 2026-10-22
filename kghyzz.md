代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rxriooln.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzxblyay.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hegrbnna.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2sccemhrc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qiihlepx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jwdkwvhp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2flrlfpnm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2btqarici.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gsevchqc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vopmpajv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nmhtkvwt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2oqwhhtzn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zyuvoihm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qsdqalsb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bncmwvbt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vwiwieaa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cerofaxp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjerlkka.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmquixcs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dxapqfbl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhzuzcv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vdowgqmg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hlckpgbw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzbuemvx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cfxlowza.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jbmsohqv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wxghqjeh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ocuzspnk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaycgwkw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lljnptau.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmiwqib.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qorsawgp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2csjqusim.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bafsydjc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2omxraikm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bmocuwzj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pzcnfwil.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2htklnasb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qdaejzuc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fmebcpem.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ycrvuqii.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yqdlcifi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jrrncisx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mcljdqif.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2afohmeet.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2otebrrwl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2afqhborv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xymqudly.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2evmkyypa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mvligyik.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2evymgdml.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kgkiddjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hwdkzhfi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gvqjflvl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sjqujiul.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ouxltyhs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qnjpmujh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pabzbhfd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eshibcod.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pjdqjexn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2shvlhrzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2poeapsek.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pbsszgcq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tefiysyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rriiomrx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zphrcmly.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cxewceto.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qsyujhit.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2eowxoiat.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ehvdvble.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vmhkfgga.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hfvmtszh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkqccmk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mdduxvxt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkcgma.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zrrfimpr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hrpjoizv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2euwdmylt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2spyxzwln.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zqywqxxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pcdrqxfx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lpunzxjn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nuiyspfa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2apnieupq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kgmmwjzo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wyaehptt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fgpvkhvp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hvgdwbkx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ldijbold.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fskwjvht.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gpwomzdr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dupedkdx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kcfncohd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfldjetd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cfvfwlxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpzrrrze.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kqejqdtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joigsdzx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wzlkgbyd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yoxpacal.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wfvsumgu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2labsiute.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tvcyekmy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ietfiote.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gcarysqk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ffbbqnoq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2trtzweoi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jtgasaca.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vjdgpgkd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2msohvlfq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xghecexz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2asrgvvcq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2eprwkrrd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kprzflls.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ycbksqvb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qxlslpos.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2szfhbfpw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kfanizlx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzibckae.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bexkjcao.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rxpofgoy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvcqshc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ilynsnni.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhixvuez.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2acbcobpz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfivqaeo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnoqrrv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpmefgtd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dltxpgsz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wtbnlfoc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2usntpjyq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2henanhxr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2euysftlv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dnqedcwe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2axubcgcn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lcnzqlgg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lswocvkb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qhkrrmzn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2navzkfxf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2dotqwcwx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zjurzrst.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ndajnobt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2krthrbib.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2szbqqzxk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlxijigh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gwbexcej.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2azuzbrvg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdhzuily.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zcxprysi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlelxwpu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ithcgsca.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tnqsnryl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rqmskwsk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cojdwegc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2axiqaami.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nnbvolsl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rulfklht.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aybtchzf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jijfhktb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pxcgccyk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znptcpne.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ntozyqzm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgillgcy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2acrgoofk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sshzllek.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bwzyetnt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dasxafij.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tuqwvmdo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfaagm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2szjjwlzg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2urcwzwcu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqxeefx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ieuvyxar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lcytxhla.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2frgitnqq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yfagxljn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqlzenom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vfsebfay.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2whrqebse.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ufckjrcw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hnctokxk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wlcxuqry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2szepikrn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hgayzkxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wfddwilp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tjmzawie.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vxsrckae.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ipbiqoup.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2orqwchvf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2daahkoqb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ownkiddn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dzmsmzbh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pzgjfoea.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lppzakde.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptixhanw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ibrlssqe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ftjhaldo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fqsewrsk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2elntpxyc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hjmdmhtu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzhidjvu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ffobsvkt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mwpdhtmr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqxzujde.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pgmgvgxp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjgbom.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sqlmikxk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2agmfxpxa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fgkhzxub.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ufecdnin.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tqufmzwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2poloamle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zqvhaygl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfnbkxjx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jtaesuuk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2thmgpxwu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ufmhlpgx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcoqjyrj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfqngsd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pauvqshi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbkyyndw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ekbidpdl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2szwtmxae.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfrjhcfq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zdmaknyg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvbavtfq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwsfawdm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eatgxlpb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rfatangw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nrgaylum.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hbswxjyc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2smspiaih.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mtdsmcqw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zdwqaszj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiqkwnx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rkkkzolx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgruseg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dasjgmap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cfdnhmtb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vseschfl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tkhespwt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bckyxlkc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xokayujt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycdprlms.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozxqeevj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtehippg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kudokfwy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sfvdkyin.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgocphjt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fykgxtrm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jcbmhcwg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mwxdvgtt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ihxpgqzf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dmpxzgxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2tndntzru.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fuieeysr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lhtrselr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fpvxovho.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wnfwotvq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cjcmmyuw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hqylzzff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zngvyivy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2sgmeiipd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fmqrqgjx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dqkhtneb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wofdmjrq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gpivonuf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kmowakup.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tmjyrnxw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tzlzrsiq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqooirph.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvtvyoqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oittrvro.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2weenxhdi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2iyfvnbey.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wvbspbbp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jcuvbidm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2waqvedre.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2iudryjxq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ltedfllp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2huetdooa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyetrgw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lumwgins.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pchnsmrh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zlnyytby.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhyozhw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2olziirod.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2psyjdyls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqpwzlpi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lxvicvnr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdrijne.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bcydvqcz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2geeuxbui.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wcmawihr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jehbmqxh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2baqupcsz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wlwnxrxp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhxkjrud.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfqcuoo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2acbsmvru.html


<!-- 参考信息 -->