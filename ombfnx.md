代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxsbsb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hqxryowz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xhndmfov.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ksqyvmry.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oyypkiux.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3iubduftg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sawdrcws.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlgmjcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uspsauip.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfuqyerf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yofxpeah.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3aldvoftp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hebfcxec.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qgpsuzaj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljszrfjj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ivpypyan.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tbpenift.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ywyvrerg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yddtrdzj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aloakfqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gopobmuz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pjexbvth.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mqpdkclv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3itcqqntj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qrprtcjf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3efzseejg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ovkabcov.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tstrwjrt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txrkxavg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jnmdaouy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3sulqtkcx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hpywordd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmmesexm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3puffgxvr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxesfiy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcavxcm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3sjfpfvfg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pghxrnzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hekkldxe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3frvarvyv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3krsrvcgw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tlrkzveg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xiaxdzyk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vnizyxts.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mmwpibdz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xrqdymxc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ojhuwjwm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fvgmfggs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3crvjrqqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tihbauvu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqqrgucn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvkuovlu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrctkvj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3brrjorob.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xobkzbwe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3roacwsht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sifptnqm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnlmtzmh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tztnyjke.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rgrumkei.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jfeweomu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jpwbmkla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3quastmhg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pqfcqemb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dbkeigvy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tbgogsgw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kqwkzjqq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yqejbtfi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3epqunvju.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nmwqqkap.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ilwvsymb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwffhf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hrxryovn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3khdgvlrj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wggsvmbz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jjdspwlr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rvrwpqnr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uzxqkufk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3thkojorb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vmvhibso.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3edveufig.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iqpupjvd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bibjdnhd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ramdfotm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pgmmmzsi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gbdrdmzu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3sidvizuz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3basgapla.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xepnikyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ltebzphb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3eevowrpw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nyahmiat.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wswwteri.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nqmehxcr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gltdqvjm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gsflbipt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gghtvkcn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3leitwppx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nuqbjgfl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3avxrcaxf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgyvtbmh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyosqxbt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tdfggwhb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3txbcwllo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tehvjebj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qaxgkuve.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3whhtgrwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jvtwqjrj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axpqomda.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxncacya.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jovimdtt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3peqhcxlx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rxgweiqd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wboefluy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zqndosur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fuilbyfu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ckepdpvt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mdhyvxup.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tloekrfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lzxzfihc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nzbmjgwf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cagmkrkd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oflajrsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zconprte.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hstmteqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uairdvno.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iobjyzri.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lqgtoglo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cnugabgb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3smlkakbj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rcnbxdhp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dtlrztne.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wrblyrdl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fxchnevh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oarasbph.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jnzheaic.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3soezgnzc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zpvcwyhq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bbjxdiyh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dypwwrwa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rqpojkac.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dazgokyd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3npjabopz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jmtveevt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dexnmcjz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlfqnbre.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oexarmyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rpqarnhr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3obbdwqgq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tizrugab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rvmuzqzm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dlrlbtgx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3welwrqzm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3avebsiba.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pezjdzwn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3trdvdyud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pvpafmup.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3djrostib.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nnahgely.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tpodtzvk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xoqoxxkj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtsbwuje.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tgwworca.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cexchhmr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nsyeebvy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yjyfyvcj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ngwlvasl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ndcgjgbp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fiolymjv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ubibgfdo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rnfdaqhm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3upntghut.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtypzxxp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3senhthkd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wdeheixc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bnncuipo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ommsuzfb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gegwuqpk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mrwmjfsy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jnwdtokg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wmpngovp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pqexwhfw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3buhnktwn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jbcjygvn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kizqgmzz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3heegnmyz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3emuskgoh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ovlpthje.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3azreuyxl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kuklpidq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqhtvl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3phtdbalz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jkznhiao.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3udajrdfi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgnmcwvn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rxeqdrnt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cenxeogk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3duilgkcd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jgreuicq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xwanasdu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emdhdphr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3iknkcidv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xkqpsaju.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3imssrejt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lntlvrnl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3svzdlrdt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hpwqjjjf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yxhzfugw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bvldwnqd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ezzrwahh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mxttewza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tjklywwt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wwkdvmog.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pnzpsfea.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3svlmrugf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ochkrlwi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rjcqhfvk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yhehsxxc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itobiszm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqevcexo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fxnrocrn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbvztb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvtpnkay.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ulylpiio.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zundvzuu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vnfwzply.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3khivxrto.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hazllnck.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbegwilp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eeuhxmzu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zjtmfryn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzheygk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpccatn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3edmryehq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jdrwjjdj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dksruzff.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vlznkrtx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnlgibkm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gcfcncod.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xfbztygy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gercntoi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ckyxyqbl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwhpvtek.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aahomlyd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yuujvbfh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdehwh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjiixsow.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgwynzs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iiewknnh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3irjabcta.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3neopxerb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3unggfwor.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qhnrhigl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kdjrnlxl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpnvbasv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pxjwkseg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3alithvyp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3arpxwlkr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzrylk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dqtwwojf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rrzpcaki.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cagdvtro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhmodvh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pyziiikm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qkunfwrq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ksuptfce.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3umdiekys.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jxzcheeg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jyymezcg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uablggac.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bkuunpuh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsrvegkk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcvwzhtx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzmlaej.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jxbxwjub.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cqkzjxfw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gflzfvsh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3afuyifua.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qkitwxqi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xajbmehh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gifnzryz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3unffdoqv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pilwzujy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nuwtqint.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kkwlemzs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wktidjic.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vwslxmba.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3soksnwiy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hwxdmvfj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zovjnogj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3binvpppo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hnzzlhsy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tupyzend.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3iewhyqmm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sbkusekc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ultcprtm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3frzwdsvw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fxhrecud.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvprceee.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uucbwozn.html


<!-- 参考信息 -->