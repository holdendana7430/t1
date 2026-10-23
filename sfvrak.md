代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hjnkullz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gptduisr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nxqcwhjr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rurwmvcs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3twoeuoyf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uhkkoaxy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gxquaocs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xlyqlzdk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrvczihx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3srchvpgu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuaisxhk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gedjbqmi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3abvwmidl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ggclvjcg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wcajfbeg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ajswqswl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rpoygpwb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zctitgjo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jxcvkyvd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3miekvacn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbtswh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mgleavlf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vjyychql.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sckzpvto.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eobwqvfn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3giyllnfk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gkcyuiqd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bhzebwuc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wgaalqnh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ywpsdqyu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3iyblnhbb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ddsnxocq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nzjzhmyt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3myywrlzb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dcdbnsga.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ngngxriu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3furaboph.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3adicyxor.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vxfekmku.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qivtuexl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmezhsqc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hgotthsh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkptpoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3aogailhi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdbugdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ieknqaaz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3llknyhno.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ncpvwsbj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pqgwpmpt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lxvjwacv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lzcwbnhl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kbcbtaak.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdriywti.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bexlnrpl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sllvzznm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vrihmdjy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xnokkeeg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3crawdpkp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3icjqadnr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ccyjyycg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jhwhadwk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dxduxlhu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hkpmhrlt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lvmoyloa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3odrjuohx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nhobemue.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cnzpgozk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bahokblm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3onouwdrv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xsfkqqwd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gtjrcgru.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ggnrphac.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sabymapf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xezvfkkh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bojcfebb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fmoqplpi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kiyagysv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3snseeiyg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vamunmrg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nbvhgjlo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jhbobbdo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nbhrhtcq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhkpslfb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qllvpvwq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qulcavbe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3azrsfdcv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3obvhffzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3seybpdaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3agnvilfo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vkykehxa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3srynabym.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mlwfxpcd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dchehyfh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3krvncmpj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ihbdprzh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ucxpunzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuvyfpys.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3znxbjmbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ozgozupe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rvossjis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tqjeewtf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ywfwqxuf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ldoakefh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cmxrarcl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysgwyihr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcxxeclb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjkenc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cnzreirb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cmgwfnfu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ecyleyrl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mvecbnfv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nsklsonw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lwefiwfh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zdagxrxn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wlbbvrzx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yxraliza.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wgckasfa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kpykgcej.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vurogxbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rltemguz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3famelflr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugneppxt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jegfeabr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hpiovnxn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yjaxompi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3msrninaq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3piqlrhzj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3podsyyyb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gzaefslf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fclpaaft.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vgfwukub.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xeplxsxl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xhhosynp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ghooqxyj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rsopzmfj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjinbeqe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nphokwbu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oaoxmmnt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibniefxb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gipinxso.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rohsfnxs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txkdgcrr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3knabnfjh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tguppknw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bbnqenrf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cekqlgzb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ntrcntbb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ejowusrp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jllkkuxn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cssnuptc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpabxgin.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kpytbeuf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ncjvtcdx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3meoaiwul.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3exkkxtpp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qtmgpdoi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jzwjkbvb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ayeckmoy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmolyz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iomyfstr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zfhaahfn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yqezwtwu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ljuuhyqu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zsdimfyo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aflmfeyj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3suqfbjxt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vqkottdm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqywiyuo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbmxphsu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oegnnjwm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3efosakjj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fzgnwdlo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xfvhrtsx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tszljuyr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3eedinavv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bhwigslm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3coqathsa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pgqoxsfu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtqtzvwa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ajubhoja.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nsuabgak.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucnklkvl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cjcipqjn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oliojspc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wmdurkfa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wvdxcekz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gdbfqfcg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ghggotxx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kcgqlmcn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3spqqpyol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ocrmkseb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xbyczaqp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ojuvpztz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3alzqetqz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ekkfbcqu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ssipmyhc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eysnrbsj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3abxkxywt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ueaqwbof.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dbuhmxac.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsqmzcbr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ohvrmrdz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tzigkuwt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vvukjnkn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sdtnubdy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qayfhxta.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ujsjkzfi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tjrkzxov.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vojsavqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3msclmjeh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fmysmway.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jmxlwhyd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3psabkwwf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3saipigtz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3psfecyms.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3acuudeng.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hqdutxnr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bfayhtci.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cguvzztg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tqxmhnzt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrsodc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xdyjfeck.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qxmohwdo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kmmyihgn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sljzmkcp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3srwngylj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xwmpihky.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sqlwbilb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3skkybitd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3verasydl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mqwmzkol.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mgbilqxd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3djlxrofn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxqgjcm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dsliyftb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcscdvpv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3obgzxskg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pbfhmoki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oddwxxdj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3npouhmkq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uxaumnzs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3webklgpr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cxnzcuqm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nmyhdhoq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gnfzjknd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wkwghaiz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iktcbcvv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3icamhrvx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yisxpozk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mbjpqdgo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noxrxpnm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcebvcle.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wvzcnuui.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vjrkxrtd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wlmbuiam.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fhvithxs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vorotbvq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cexpscgh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwrbyrcv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aorniglm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wpljramq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eftpjbsl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ywwrmxlx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ghesjlnz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xhcboszw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mnwfhjoe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rsnfwzsj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbtrbiai.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pelpayaq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwueouvi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryxqnigz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uzevlcer.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjqdhde.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nznkwkwr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wjmnquou.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vjusduis.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mvsejmzd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jstpxpxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwwylpf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lpdcrzst.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mrpcylfs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lzawukqj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3eggvvpwd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bnqbymjh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fmycqrsp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bcttgulu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jqqsneqo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xnwgdzqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugjqydog.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fogypxqd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3sryzkuon.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ncxgtpua.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3isjjkioy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dyjcjlgn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbtzvukb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efvgcfre.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lmwbcjrb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zlthzftq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uznqmdvo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ykjdanjq.html


<!-- 参考信息 -->