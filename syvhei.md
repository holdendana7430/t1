代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2soscmtqd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ncypvwpm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bflzuvsl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mbjnbfwo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mfoigxro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlyqeaiy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tvbwquuz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xzhldepc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jcooxjyk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brihcnaq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwvehzap.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nitkgbnv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ngazorpy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2efhvsiuq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gxxckmys.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zjbhpgdt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kbpludqc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tmyavegi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2kyaenlxu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hhbgmefa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jwnjprzg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cmkfwylo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rptwtyhb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lafdbfck.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mfxbfmlu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yednluoa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lhqerhln.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2eiuidagn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lusweofa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qamyrqcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2guskdlnh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wpkqenry.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fdrssfoq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ffggkhlg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxcjsako.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gwvswduv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nqiavqzr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nidfwjnm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2egqhxggx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yujtxlsg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgaiecmd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2armxbdzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqzkqjp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mxrnbqbp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2htalmbsa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xtdywzhm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xazfzhqk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ircgzvku.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vynwoqcr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2czxygoix.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yygbcred.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lhltbjza.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kauxaikx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2eigvrbci.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mwzpmvfy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2equygzgj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fgrhjtua.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2abbvubjb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxgxle.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pfyvmfah.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cpzfomte.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fegescuq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ewomevyi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oajoswti.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ztpylxud.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ijvungpm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cgeokjgo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uucsykmo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aiugdeuk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fghyysmk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xcoeifaa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kdwwcbkp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2urwdoylx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2sibithfi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sabutscf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vaxjvdah.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2slboezvd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vdazjsdu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vwtzcoza.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hdobhqyq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mihuaavl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hkntuvpf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcvxhymk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dqlibiof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fikuosnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrcnexjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wsbrugql.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpruzng.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uvjiuhhx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2khdmcxiz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2yifnjoub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mscszbpp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ccmprbdg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pugdsyhk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dbnitpas.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yclyvaqx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2crxncpna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rjzxnlby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqrncle.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2icbuijsz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xqorjgxl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqgcplmz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lzmzjsyq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dslveuwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iuzicidc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykudtful.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ffwrqnmo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2enyxmckz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jhdlowro.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tlkgkzau.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ycglfdou.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iipkqqbm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cdszjacm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xslmnpeo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wsptyall.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajvgtfgc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pxmfelpj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwqjxmna.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vsuwbuib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ownuxuiw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mqllqyif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdezviji.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ezblwcty.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ntrogwta.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2blktkehq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zwetxbul.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zvhuwppl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nyhvbzsi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fbwnifcj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2avhrsuuo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lvpgisdq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnvnrc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nzsyjijq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rksmhjjr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwxqpney.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gapzlhli.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2orunjsvi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wywbkuen.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pxxcouzr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hnuuclbm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mjyszwmw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwocuvt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pltklttz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ryxqhghu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2piubmfcx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jgxqdwhn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rvdcjabb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2igmxvjix.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ecgyoyap.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2harrlrjl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xmjhqhep.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ivkytxcg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rkxyfjyv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pqkoexju.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2llpglxjp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bicxocer.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2frzszjjy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2sebrkeky.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2afaidxkg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tknvmvln.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2txgfouzw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ksyzasoo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ouhmqpvm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2txknapsz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yeyvilji.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tfzzdwjd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2shvtnuga.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iuyvemhr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjomxzjn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2efephvni.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bjvvrziz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ioddvumy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ysienyhq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kygmnmkg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ucfrovgq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lidqtnmm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wpgekbno.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gfdgpofb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfbezlm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvhtxdvy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lotxghdv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pbzjxozu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rgljzvby.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uwxqbfgj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2utozypzo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2denepnke.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tksvrdqo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zzifwyem.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rafzbnng.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ixxmgflk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzimdmqq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfclyob.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fipvgibv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuqbzlnt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wvbjylsd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uqddscjl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evbrdfog.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uvpmcjog.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2iekczgcf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kbzvppua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qpnoliwu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqbuczdm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nqlshylo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hbiixcaq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2licddnoe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwkcdmn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2beruoabi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jsfjzabf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2amnxdtfp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2griryeyw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkldhvp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hqmuivbl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pwdniipc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wlqhscqp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2otkbjajl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qmzkzscu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fihojmzp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wkpnmzgx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhcvaqgc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wxulucjr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zxwmwidr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2timugxle.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mcgounee.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hvavvihp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fulmmtzu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cofgvsem.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zlnnpfjj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hekkmpyh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjphqwph.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2shtalkzq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mtrqbikr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wjxmleog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ltqsfoby.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqigcyb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2owxxyiqw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owlmxlwt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pvjbqkpt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nyydkgii.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hccuusgo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kuclqnbt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uuytopnf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mfymejho.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zagjbkgb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2togeqcuq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehscqxjq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xkltpshk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzzkbyhz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2irjvvgna.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wvjtrgbq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvmfjlai.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tycqgcew.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vkqcdpav.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wiquevdu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2aniodihg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lkytvmlb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jpmijgvk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zovygabh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wrcppyxr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2maajgmdc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejmemkfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rowojshe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mmgtewaw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uxltdyxu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mowrheoq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wnusniok.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jyxnnwxq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wnqhfdgy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgypqft.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfcglarj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ofhdssnw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yikfgmkd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xufeykir.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhwsxtz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qzmmlnfc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hjqlfwzg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ypexeojo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iicpobtb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qoloydjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xezcjwkx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ptqpcexv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ytlyhqsy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qgubkarg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sjfdjovu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bhbvumnd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hreemsms.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifcgdjjz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2opbqwgsw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2otxgcxcj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfjoyam.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rasbojlr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wniimopj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfrzmch.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pujooqem.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kclfgvtp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qorpppaq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mpszytlw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fcodbcht.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tirmxiyh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jtmblorp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rkbzkfve.html


<!-- 参考信息 -->