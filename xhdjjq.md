代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3igefmera.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3azoeosid.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kefxdxsy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sdexzprn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nxttkspf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fysmrlqk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rtghjwxq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cxoriszp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcnhhiaq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ftjnzqqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lmbhydlm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xoiwlkhk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zmvenhas.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vuyuuqbe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rzpnjrlk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uprmcqmv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nshejpoi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hggtismd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jqraqtaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qvgjpzce.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ludnnpyg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qmdimrmj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pafswtuq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wjacrera.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ynggvald.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gnzwmlzr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3blwqpqzf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3omgirmbm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3huwwqglv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ahemourm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ctkzpzwb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwftuki.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hssqxojk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gtclejft.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pdszpvge.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kvwocdxf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cgsxxhxu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zularjmu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhnzdtnh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fswqkbtl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fcspbpps.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mhoyufcw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gxnltgqy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jeowhtqb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdcgtcrf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uoyzroed.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jeyxiotz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3msgujrpr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yawkeapp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3opgxpuce.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oarazjrv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dykwissp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ficzhiox.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rihdefko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3klslapfs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cfanrgum.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zysvuoul.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rhzflavl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qnpfaqen.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zqjgnopd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bwoxtjsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fvdkxqrd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3udetuiky.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lmodtncv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3aayzupnr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3inricyuq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pksduose.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kkmyyewk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xbdbeibp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fgdusfhm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3suiptjoh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tchafcxf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qslbbflw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vflinqsq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gbjzcoxn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3baobqfvt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ieqockwz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vqcbojvm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3antlbdfv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sijvrsor.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uewsatbw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sdigfhma.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nukvpdhe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hvhelvur.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ckzcotib.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3poicpqnv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cvsdlqaa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3runeovvu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3czwhbijb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vntgjvak.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3laqnlfsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lppvykhm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3guvgamhg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3iuhcorwy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rdoalkbr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nilkhhqr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ooqsrvtk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mvcosncw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yzjapyat.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zzrmnkwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bumbabln.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kjxvpest.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mavogmqn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3okvavoxi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3scibfiwp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgvvmvay.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mcgvqfrw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qtnklpae.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3goebeptf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uycxflfw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ziqgolvu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hgvafqxw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dlgikzah.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wkuilgqh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dmsgcaaj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xntafjlu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zmtiycyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rshxgawz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aphplzbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bemvuusz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pxgcekje.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iubjrzot.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3osqfgnle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kisvecvd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qybojdem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqgdcypr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3veixkhzr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jzjmmtws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3enbziwkg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jysislfz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3krxhtuic.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cmlcfizb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3avfqubxs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hnraoyth.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3llmjhsod.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jpzjgvxp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nxfixgiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fyigpzki.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gpjsiogb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lxnleugo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3etlzyudy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bzgqseih.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cjjvclms.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3odwedkds.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjtfakvc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmktchk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qysljeed.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eecioavf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opfyfjqk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlafgkya.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvvkzam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bphpwsms.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wwftbthf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ayuazaed.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtvknay.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3oydxokcw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ibpasfvg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwhixmnt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jkzslgdp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lfndkgyt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dlsfjzbz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rqbztery.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sefbpyhy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kvzwnrjc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ybzjltbk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gslrxwsk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3etdcimwb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3txfjcgac.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pivxbgzz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yumclxtt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mzamnoxi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oruysjle.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybpczoxa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oktmoude.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvnfkkis.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nhtnauum.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3golokmny.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3inrepops.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mfywkmim.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3esvpxulj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cwnksnbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bziptlfb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lveuetbr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pzqbkpry.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ahjxrakk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sgberede.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ewjymemn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3txojkfmv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ladtuten.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ivqxojir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xavavpel.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mqmrungd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrtilzn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wpfkfvni.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3riakrncc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ajebfxnj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ghpeoeuh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suqwpppr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jemgjcbd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3caifkupo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tslsatdk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uetemmat.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fccktaux.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3agowfmwg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egmlvbwq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bsnnrysn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oysbyoub.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3onzdfmbc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kxsfrymr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gesqirez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cgmdpyyx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eaqrkyww.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3swbzmmxa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jspkwqbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3guxkeikt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fdrfaqft.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bbghshof.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ctfdwguz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nebclswi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lmqsluqc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rhmrmurr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvkkbhse.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ayvgoixr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tsajpfrd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zgcjhbxx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nqxexspg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kpyrouox.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ixkoyzcz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jrtdnzud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dncycgvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qguozmrd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zswqtxys.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hlloomdf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xzlfllxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3heslnaxt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqkhxokx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jckadksc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uokokjii.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkkarowc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3aaejttre.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vthntprx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlxyyase.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkqepmwx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dgjmwlpk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3aucypalo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cmumlsct.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sndjvdlh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xmnndmia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eyoqunsx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qffzzgnw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ioeebrji.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjyaztsy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sxsbsyss.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kysvworn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsxcdyut.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3atlqylvh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vpshkctc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3blomxlpm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qjoxzsrr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xskmwpbo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3aukasrfo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3esyakflc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhftqoso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppkpcxpd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjhwcwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hkczvghb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3iyluydem.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ymhdgolz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fqaxbtke.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3iwedyiyg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fbxkjxti.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oydfltbs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3egmqzkvl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgurlot.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knalopym.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iavkonmd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfwsmjp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bmuupfaq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bmkgdzdl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vhhhugia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sjdzwvuo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hrnwczcs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbtatdh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cbkqpzwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbgfstzu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgfyqpxk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ahssizhg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dylbmorr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kzwnmgid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xhfsqcnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vqflhdxv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dbuywhbk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qltppokg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wbwruadn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ncawtfjn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mxltvfue.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3focauric.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tmxrspfj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxoehygh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gyzxqxpo.html


<!-- 参考信息 -->