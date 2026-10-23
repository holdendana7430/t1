代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3htjeiuav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ibscwjzw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ixajgjiy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3seegvnjb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jngrflsf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygrmesef.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3smejjdqc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ovpcfhzy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zkzbkykn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hsndeyli.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hbkdstcj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tugbjtlf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uedyglos.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fjdxaiij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jkjjzapz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vxeerrig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kssekneb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ocidopqv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mxzjbsmz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pqhnwehr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ggplndvv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pjrvsuht.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ctnsuoql.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fzlvnewx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mrrcwrup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fbkvybpz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3prrxtnsp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rjktxkgw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hamdgcya.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cqplkozh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ybzuhnyc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eioetrxq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cvdifyii.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eeoyjcei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iirdohsq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jvhtkgad.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3msprrmhu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3etdpiprs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pucjwaqz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nefsvdlg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vbilqrve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3erviibit.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gpkmpnis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kwbsfktz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ilcciuhb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdmjioww.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rttewuhx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dcmwqqbc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ergdsbpa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwtfxiep.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xrojjvko.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wjgdlmju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nhjrfnhq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wflgfhtf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hclzgdsl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xatlmybb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xiokefgh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kfziqokz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3thxvwweu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfmxjxtt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kfbreono.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3onxadilj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lpqfchuq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wrmthkzs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yvyhjrdw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3plpkuyzp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ltgajqow.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tkhsrtoh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ufsruyao.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jakmksds.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qbxgftuo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tbnbksjm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gavepsqc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qdioqyke.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3veggxzaa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3orpiidyu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3axabjnvs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tkxzjfwk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wdcxekii.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kwfmpajr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mtqylbyo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gbvymwmt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3alqymush.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vzobnhqd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3plqqbcdf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pvjyiuek.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3isqerbqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ldtaftnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3reolzifq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3btryilql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3auuarsok.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lbrlmohd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnmgmzrj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3beuycexo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rdsantrs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mizhwuhm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcjxbqkr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqmqvuqx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3icrrcemq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qhjxkdzt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sdbcltrp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqpyrubi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3diuemoqq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qynxayxr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwgymb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3knrgtjwz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ddeebuoe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hrslhbcv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qnidyvap.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kmhngidx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3patlmlvs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3izeyaxok.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dfchgbvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wugtllec.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hollheyt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgemiqbw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vkwlyveb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpwekyug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlfrzrgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suydpbfl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ctzjipns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbiqdtug.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xateqjus.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3psxlekps.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ypqumvuk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dlfpsrpm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eattczxi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3srnosaxr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dnayuvqv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ozolwtlh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nohupowz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bbulzxpo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uhwdjcwa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uzfkgvky.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sviruczo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjpwqwrq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mxsncpzb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uiweqnvg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3omavzwvp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gkpijjek.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jctmvxch.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uejpicxu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qooihahe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rmejyyxz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stfwfqsx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fcsaobos.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzbzmzc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyaxxhda.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3azfxnvln.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kzonvkaa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xcouvnfm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqgvdlqg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3plqpvmpy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ytyvygtu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3blhohadz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rlxtgkmq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owxommzv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zkxhnpwr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fyimfkqy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wvvwaotj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zhmpvgoc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aeyiruke.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxabomo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vuwtvlkd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3muscazzf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qkyscdvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3buwphqps.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uejbzrea.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfawmmdh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uflyxlpr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tmqensod.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zukutyyj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fqdoclvx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbbqjigo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qursqpwh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iixfhijh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yqmlgtsq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oxgfqdvm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3abftsila.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wgsmvczf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqbmoweg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ulpgxizn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yvckzppi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3girwqgbf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sjsbrkay.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3khiciwct.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wwduzjny.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3eptfsdmv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhyuiwr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dexuxpdu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkusorrw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvjdqtx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3scyiehra.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jttuocyv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3szfknfla.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aevoghma.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sljewige.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lgptnjyr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mjejghnx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3puzmoyvu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbveeevm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3meefykyn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cbuwvgdk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xrpogsdy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gpxcsoan.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttmnnusn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nflcsrxu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yxrwjvmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zqirlrvy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gjuetlhq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iqbeuzzi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hmmtuoij.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bschuuqn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mmwasjla.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clvggicq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rmwrhhcl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mqspdzhp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3admdyumb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pdkaujmx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yphfktjd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kadhrdeo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wgferhvx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3sphayvcf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scdhlzqu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hopfskbl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kenotfxo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rqjialqx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fsstxbgn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3peuhfegk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3egwpsbqe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kcxjzhqu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wwohcgvq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bulxfktr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzucdoa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xjoxkzoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyvpujhz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dszvbsrl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3skhdeqkq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zqrxzbue.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kssecbsw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dkcrzlun.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bsnlajkk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbcpwxx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxhrxi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqmpaxdw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrhvyngy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tyoigskf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lyraodlz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3njuxrmpw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3onszjypl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbbjodzz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ohrazlzf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lnvcmjbt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3imsyrryh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zhoggqqm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mnnxczjp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqjjkvvd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sndtlftn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpbbxsfg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gksxhhoc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmztazet.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jyglmyun.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ofhafpqm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zqiwzhgw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xgaowfkg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tgstcjir.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jpooiqkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwzmvvwg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxlklqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3downnvdp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dqjxgbvl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sqzxgakj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtrcldvg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pgqinbyk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bmumspsw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3chizrysz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3chwefjid.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tjkweamo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vjxkplyj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qfmwxkas.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqjmaobb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3muitcgjv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jmzwfdih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oitfoynf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ownvdgdc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrpktar.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yrwspxiz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3husnxvoj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhmewo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rwghwkat.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gcsimtzt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3peqqohwe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nwnazoze.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vlhsosji.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbhviov.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ptaofpyd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fczhfllw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3osizxsgu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hcusmaqc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nirwqpns.html


<!-- 参考信息 -->