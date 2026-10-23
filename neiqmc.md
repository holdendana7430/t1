代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oufbzjdc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3akwmitle.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wqrpxutb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrkkckv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxccmm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qorfpdig.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wrxgzaxb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rufrhvxe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkohapxr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruphtmrz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jnhzpxxy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cdykstzj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ekkcxnni.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ajmvidal.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3maewsrle.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tiyzxumr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qxrqvske.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gvpqsjhy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xqnrjtou.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hwoollvy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hopxvoja.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sazfuusw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fewjxowm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3naidjhuf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vkryyojp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jymvispc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vjtnlwbn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gxiunpcz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qpuhbmfi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sobemjtp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tobtqaek.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrvzhghi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3euhuipju.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3viemycuc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cjftxpbx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3engqfiqr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fbdelpdc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3nlvjokqb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dvrvvcai.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xlblwlkg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwnmkat.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qcsrfwyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xrlkdhsu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iazspwec.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpwexpnt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mjrenbav.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdvqpkk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3icklfucv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jikyfxbj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpgoorzx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nbylbdau.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nzzpnbug.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmgersh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ygqkezds.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnudzzq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwuzphhs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3stfzoxug.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dxlmcpxb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3peaykyrt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lqufkwuc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gmwfslph.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lrvitowc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wfyqzutd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cjjznvdv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3duhxosuk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jcwmiffr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wfiquwlo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bsbhfenw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aovmbhfv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cromkedv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lpeiarrj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oepeidzi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jxpuzcqh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ryxnmdqq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hqnadxhn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ywhnmigu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nsxscbkf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kbrdvhvg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3urhefoja.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jdbgrvop.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gnclmmje.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3swjprxgw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqsaqwhf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ouitblec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ewfwczwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rqkdmoxc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vuwhvrmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3omyelqhm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mcwrhuxw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vfresmov.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wnkihbgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qbytheyf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjxrlxsm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gpovxpcf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qmedfxnk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3omcihvcp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlcpbeop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfyhjok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lafkyryq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vqwwyzwq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pmwrrcpg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xvximbcq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wvnuuygq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qzllosvl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdyasfsd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xicnrzvv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ecndzjxs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3anggqeey.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qjttiguk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cvxuxrho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wsljewsl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3smkrcsob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cwxhzbci.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3aoniwcyt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bvtskcvw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3njoygrjo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3miksmevi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zursepnb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3eiievtfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atelwylq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zxgjcabn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruzjcuqz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lvyunolc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3oirdiixr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3afjtmstz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xucydvgy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tpdeqqum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3knwqnfwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvtlfu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hqcrisab.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3imoakuec.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nouymths.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3trovpypu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bqhyjspb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynujmjte.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ywzjvirv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljtuurwu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wovrhaow.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fovgynqs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pziweqrq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gvadoolc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jejqpmzk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jsloihbv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vbvejaiv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3spshholi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xwgzqtym.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ylzyjcol.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3usfvcemv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hqvgkhsj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cafesfpz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vwafbcat.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sngpgnsq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkdone.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ecduqzoc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iwojuniz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3agqwgpur.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3klrsshli.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vorgxuee.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vdkaqntj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rtxieuwj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sozqhzag.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yqtooxxh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnslxqp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3brptsfwe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vhhmxfan.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ltokcczc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wpjxnjka.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3opxiklak.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3klnqoiog.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ondjlvwr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qbvivxse.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uhwvmauo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3uwozlywr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgvzvqti.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qtizjuck.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xpukepbs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rzxsgfpv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ctnudxic.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pfoepmlp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdsibobl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hvlicbdp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghpnmvnk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gnvsfbil.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3djlhgyxx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rlwtlaza.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dziocmjb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dhrbawgl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ydfqvaag.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rgvivpey.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mtqaqdsh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ozyckgva.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxawpgs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnrnhqht.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bddzugih.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3itxfmewc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zfercdkj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gerhastd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jgwmdfkg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lnkjxask.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lnjptcru.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nitsmwpx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3agseklak.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wnghrxhv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nyeeinim.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbbrzia.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdoxpvct.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zohvfwll.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vrabhfrm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ooygcgud.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uxdmvfnv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mmqymwzj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ajcawosc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pgqlfyrs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3duqdoftm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3carzkgns.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3udrvugbs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vgdvncrw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wfmxvcyr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkpdogz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oqqrjven.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kcjybzkm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wxxfrbhk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tmdqenct.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3clqnrgxw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsubjai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnifxtj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zmcsgwsx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozuopvcj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3laqbdqnq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vfmurgly.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mrqdgfju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qxifqtzf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gztelmcg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xvaxlevm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyvyssg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ynknxtld.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3piqwhrss.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vnorafsq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kysvuvwo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xwakoihf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hzenkylg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pabevsmv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zhgcugkl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqcavtyd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3izesjetm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3suelxbmh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3llacnuvf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blrinqbu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3airazvhx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mkhfytyu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrpgzeja.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kmvydpgk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vzdwkxoo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3clzobhks.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mzcdrxqt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gwrayuwq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3raioymgp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3usfnuegq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdxhrfsr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqcofbnd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfsmxbt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3puwpwmon.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cxdxzesn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3elqqffjn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ytigjycc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xgqadqks.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gxhfdqgp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqibafxn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3shqxhfqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jfjstvkq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pqckpyxq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vgpidooc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elsepvwx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xumrwgix.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pwtyupyc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nwyxyags.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rdnxhkos.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3paagiouv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ynupgkqa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jnevptep.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gggayiea.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3osgyecsg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jhfezioj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bhhiqzaz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3snewtsqm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rzfbcvxd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kivzkyyc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mynfemal.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3raurnlsb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zcvkiusr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yqjgigiv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nszqtzef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yggzdtok.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dkowvocf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldgdilpz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dgddzxbc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eqdenisu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3timslllo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yzpwnsvz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kgcktnrn.html


<!-- 参考信息 -->