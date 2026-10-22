代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kcggnwuq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jukqgvnj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqzsrijl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nrbvbeff.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gtsfxuug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fdsjsmuc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fkyqngeh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zcqhclgr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxcsmgnm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zahplqai.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gwyhmtzx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2decpqxxu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cksyhlni.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wfgrkfft.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lapjckzq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2utqrnilh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cnzzpqox.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qtaetrdf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2chqriacr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2eyickzva.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rqlowzkt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2umehbczj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rkeryqxc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vtmynuyl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wiabzaup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ckezhwwq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ghplfjif.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lqdvlgxg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lojhkchx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2smtysyck.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gvdbyvrh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zqsmorvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2obruuyth.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lfidaoja.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gsstnupz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rripntao.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gjcyqukt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2whlszjxb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2epstzdgn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nagptzbq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ggmfvufe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoijzqyf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmsmyuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cpxsdwlw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uccnpgxy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zofqwxwm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtybbuzr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2opiakibg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mmrbrbul.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hfsvtwjs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tjrzblhf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lfivcduu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uuqcfpph.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jscyqnqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzjdhook.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pjzkearu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gbajhhwz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dtgvxqmd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ozplxugb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fmkucuwi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ntsrczjb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gjahlrup.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ofxyyjsr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dagocdir.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tuwsbkvc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bimcsodq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bcobfifa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xpjivadt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ymyilhuy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2unlceysg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pwafkdae.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2slubzxrq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rhcczthy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fuvfztdo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcurrn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wbwhkzwn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tajwqsca.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bxgdzkuv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yfbdxvqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hqglhzqp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ggdrvsut.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2brpuhxsl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmuemf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nrvmywgv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2truyudyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qmeshkkh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2semqnwwm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhlgmnj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdqdvjv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwtset.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zsnywjhn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kvtbowha.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nxtawvop.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iuepnwaq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2makummrb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jocgpbnf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2eosehroq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyvukjyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqdmyaj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uctkvrzy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zklncmpe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xyirgqzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2anilijoj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2meszhyoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsljqjzw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcejoxod.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wdyfubic.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mjxmvxql.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dnsucdtg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ipgavvch.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lgustcln.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mkbttwnn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cedftkxw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2khgktydy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kejlmufn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qufovycv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2goslmxuq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qhemghmu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kmcclsck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tglszjfk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kamwpbyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2durrdryq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ojexqhzy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hyzowxlf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wimemzop.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dihpbpau.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mggyjjcp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2huhbhyda.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2idzhsopd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mdrydmgo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ybccjmpi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zjaapxgl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2amrjovyi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zzlusuqm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujlgtiix.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2peruynew.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmltzksf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jrdkpddy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2odnasckd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yrwvwbxx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hsdluiwg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrwsctm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ooeivgss.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cemuuiij.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vemhpuom.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tvbydauk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ckpcotco.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kakxgybg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bulcnpdh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2uuswtwkc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yotuyulb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znwncjks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2umlmnfqo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rggwqwos.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2boooukmx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gauicuop.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2djvjlhnl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2txdaejvg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2airngnfp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pfyoexrd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gqvzvfct.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mnnzorfy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aycuzyni.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bphkjwgb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nhtlvufp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hbmporls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2elxwvyxv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2volhindz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqqdjj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hinqpxxn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2liqmbvmn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iljdlfkz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yepzhoya.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrxmrfya.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2twdmspfi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2swjrkztz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2arlcutdl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ehaetomm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzcdfhq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zzvqmnan.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pigtslpc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2njawxkib.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ptewdboq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ygtmwofa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wasfyebf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozwckway.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjisdxcs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fyeknwnq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iepuwfba.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wbiwxusy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cxiazbqr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2idmcpfsh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mgtavftn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yykuicwl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2knyidjjb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mdbuwpym.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrrjemoz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2byjmujgc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pstvslsq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nxelrkux.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptupkpps.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eomublza.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lfgtgsqz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nhddbhrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rkewlezh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ebckojnr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxoakbn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nxoyghpd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lmtbkdzm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2krntxfne.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2snxectak.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mmlannea.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wlrqlodk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dntqhvhg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kmesjhre.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ridlvwxw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zxyywwno.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2crjrgvef.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oldpjrrs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ltsbeloe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pdqyngsb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2iicsdhpb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gvczaaxl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znuuvipr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gtpyseou.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cacmcwiy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mjutcapu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsxjvdt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynedxraf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kxyblafo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2flhkfxzy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rnliwpze.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvisstjj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqytoijm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvazewwd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkerzvvp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pouyufte.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mszuuitq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nctnxhor.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gybfzjqy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iqtsxjfs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pqarmbva.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlujznge.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mwkxgyzf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2umnjsofl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ixqkurvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vzuxknmb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnqqhtzr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ouesozke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2radqgmpm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtifqcoa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bxvxcgwv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tilqrlxh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qphmsdnp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rkspejwj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ioxihdni.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qervtmzn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bwozzdrh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtcquau.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xypcdzru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2natwemzq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2umvruhpi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2easndpof.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qofvmtdh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jvcxgofk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wwlrqify.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vzrtnteu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxonwakj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwgqcfae.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fnqpyzvg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aoqcmgds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2oforjbqa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2trvpubdb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fpmyxvjw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wmoinqkz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lptuqngh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2endmltui.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ijxahjgx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2aasypnbp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iuwmkpyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgwwtsus.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zozwhmoq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mzmntmne.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtzqauts.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bqeeyoyn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cmronxbt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xwmutvbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nppyyyaj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wajmljil.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tnsixdze.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2slxqxnrh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2adxfwcjg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ooqmgmhe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hcupqvmr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmlajtpt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dnkgycvm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nkeypmue.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dltkprjp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wlobrnbg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yvbickkb.html


<!-- 参考信息 -->