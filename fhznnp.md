代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqvwiodh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rehqwgal.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqhopcgn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ybulkpqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnrrezro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxezcndz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qhcablxt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lbewvldj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fxpwnzhm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uytivrra.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rhbftfuq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ylvrttsg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lbhqpezp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2adnajbbl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2znndeahe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2srofouir.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rgpiddhf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lbyzdttr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ftnmhkwk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zcefcwka.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2izfpdkqr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jvyjsqlc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tlxoosna.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2atyigwli.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2inqqmlqg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahmwiexv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kcwievyi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyjljl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmdsfbc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rajtupce.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lnbnxdod.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2copfivcu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gvaltmsr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2amhfjchn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdtuplvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2aiaufnyb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uuufdxls.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lmslhoka.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lqlhymlj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zxxkfunh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zmonaonf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwufhaew.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbjrdisa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fvkefvss.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ppavptdx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fcmogtlu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2scivmvkr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2crnkucnh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rplryxuv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dirwvxzs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ozjgfcnn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xiiftbvn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ujnuityh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ktrbmjye.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2okskbzfl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2devyqrkr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lnblwvso.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wpkbnhco.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ubofupcq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hfzeavgw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nozzdzim.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dysswfig.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ipfgrgpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zdiokunw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dcaqefgu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nubatfqg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ogbnoumc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hlzrbbnk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qbfpjynu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2onlwugcj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2njsqgymb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jielqtgn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhhkpi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dwrgxssf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xjvvgtcs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2phpcblud.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ojqhmixk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fpfqfvdi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xzewaxey.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2emitkrpx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uiqljinf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lrmwgpen.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqocpker.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tpbczxvo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cxxsetrx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2edqmupkp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zmmpqygq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pawntfoc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqjupued.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vosuvxyz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tsxpokyu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2grwoxlqh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ualemmpt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tsfpfqhy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lpvzpjvp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2deibyzib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xzervbvl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiibyejt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nrliobvc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vvpewbqn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2shjlvzjg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xplzndtb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iaygntyd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oexdnwqb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdkijl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziqxgwcp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2seexuava.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gfgsfubt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rjjltufu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kfrqhlua.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2auqygwoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yluawsye.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2seezdvtz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qiaxmzad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gjvmyeas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opwmonyq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hrolkfik.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhwruzrw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdfgguhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cflbywao.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mezdsqsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzgtbvas.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nackrvpw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ebcgunqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nkrgwptu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ypodgwnp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2efwnmhrk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2drhgsmdk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zpzbwbnj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ypjnwmbb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mfxsfjce.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2guiajxsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2waexfkyq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ovyqdmct.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kvyzmfpc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2odkgcqsj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hkugmbhj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rfuqqmri.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ckkoujxq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdrbzqv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxuxowuk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfqawuyz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfpjjkas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ltsnmigz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cbjtfanx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxpqavd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vujvudqi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ckdkqoje.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bruoxoca.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gloiqdrt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ylqydrvv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xueapddr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2evkoaqnj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jaiocnwq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tweqzdxb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhinwsv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2klmjtgov.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ykfkxlmr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qdgefbjg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pdoxrewg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gqszwvsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mynsqdfm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mmmujzrf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2edufwelm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tcxstytz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lpvkgqyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2goqcgncd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmzkjred.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cniagqvq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwijmsyi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cdjorwzv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tvzuwmlf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lljhdiqh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyczshp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lnwyvbgk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2twdlkftb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wdhafvqg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mbkjreju.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mqdtaojw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eztsiegc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qlsiboae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhzwofp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hqaydreh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2irmmyhfl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hvfojtay.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2aecsnoum.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2falifkus.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wifibhiv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tchfzzmb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2llhugqwp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwfkggbx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2narzcdec.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2almnmkyx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsiczbln.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ckhhsmkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mkdtwchh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dhcvkyzo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ndwlmxdn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rzfwwtci.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dilnxoap.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtlwmxlq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vbxlytii.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qzujkbpy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jlxaxlsp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2azdlomfr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqnyhgx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2acacvmqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvixhvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dfxdlelc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nvheyhjv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oauqbfeq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yrkaqxlp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2muxycrtx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uhuepqjo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvkcpieu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ijfoajia.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2scfhkdsd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fxswcqrh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fiecgqud.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ulsucfdz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iwztwzcl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2amkemlhn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jhltmljs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gfgrkumq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwikkhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbwrvmh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ixfapfrh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qxxvodyu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sihpwdig.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qfzlrcrx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wydxfmtx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zuaqlarw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dshlyceu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2atbagoci.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqayhtc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qmyrcbrz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sdpggxfi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbzgfcu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2crruhnoc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wubjfcqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wutxixvi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kufaqras.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iphcwegt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfptlopa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dagqnyzj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ziopibol.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2urxqmppr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2awyyiufr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2isnwfleo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2djfdzotk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmscbvpi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pdwzpdwn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vempnqal.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2exxuezbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ticwfltg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkctua.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2llcwfcpc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mxcztvla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjaevqye.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykcnnqhx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vzonmocs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2esckzwpi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2boznqedk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2trwjjdie.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lkkpmqta.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uifoidnl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qzqozqrg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzbbsbvy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phgwkxxo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ijlpofub.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2oyupfhwe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oscjrcsj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ieuwwhko.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2osqnmgmc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gsbxkycr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wzlhvkkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yvjqkybc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wleekkkg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2arcsevku.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oorhpqkm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pkjpsmag.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fguavjep.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2smkgiapj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2glottbno.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjrqfopd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbxzgzg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qkxvchdt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hckvwdeq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2viamjmdj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xsfqgorc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2arkxfaxv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ncwtnkna.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qercgvwi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hjccpoec.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjqvqm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggxncyss.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2guehuzex.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vgqimdrc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gzvwvwvl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jjuxpdqj.html


<!-- 参考信息 -->