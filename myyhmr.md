代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hlmwcjne.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qtmjdxxl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ysbrvwdi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rbyumnfu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cjpsasqs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ductcpzx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3sguxjaks.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jzknzoor.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mocdamqn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ayhklhme.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yugkonpj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xmwyakyh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3igkibgwz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vsxldvld.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zsofeyhe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukypsfwr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ekizjabq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrdsgv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3psennrmz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3femqfggn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3srltcuwx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ncqnmxjq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ucssjtpg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ohezxkgy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymfuitey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mthfhvxl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfaccbim.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3oarxwqgn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qpfgvxfd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzreaptx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzuywilb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ebqqciuj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jzebbosy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3seomvltw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3eielncdb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dljiwdwz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hknzbocf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcdodppd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcraqoxi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vuoqkvbs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qxpbmtph.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3sivfwdfb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bwehcjbk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pgmawbxh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iolzpezo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dtmbjeon.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jvjrljup.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ttefuzxp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzlfzruh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3joriqydj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vgldumda.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3psqsvtdg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xodqanwd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ipnvoxqw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zylhvcon.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzseby.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mwommbmo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pmjwimjl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wjfseumx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hfagblnm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fizckped.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3unbdocra.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jrosxhrx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3eujtzoao.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3usdbpnjt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pxsujmmg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ozghjmtp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gtreukwz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xuvonxpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3runpfjfp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3scifertm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwafcdn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3trsjqucc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tmessxhe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3imwvbmum.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qqxjfydf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cahslpcl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jceezyuo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gohuuybr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eulnzmpu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3umjniqak.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zordqreh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwlbgm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mflcxpub.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cpyocdkq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qgucqdzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kroifsjq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3saposmmb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvamoexg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tegrcwrf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3twltuwvg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmodsi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hkwfyrnr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mxlkrpig.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ipuobaus.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3diiwtbys.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jmfobsbr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eshauzqc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfmbsqpk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmaprtct.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uyhdjfpq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxswhdir.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azzwjztv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmaivpey.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3obbvwcfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojtcqzye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tmfqklaf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zhdvfdqv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dhmwhaah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3himokbif.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eweuuyhu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3btutrwnf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uvxzblqb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tvdacjjv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rjbwkuqo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fgkvxhgy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3whchceep.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dnwgjcpc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3djbvqzro.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hyedfwgp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3altugdan.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xtkyicmm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nupmnxes.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pyeeekex.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kftxyuxj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xuafgujz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3imnyohcg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bjkwjbks.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yldxqrvo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlccpwog.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qplsepjx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3emcwtxpi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3agqhgxnp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dfsgpybh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3shxvvwjd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjoefgna.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ssgjtbjd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yndlmuxk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfsgoeun.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dcehckms.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elmgksij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaxfdfgi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qnmwfkhj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ubwimche.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3advsurlj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oupgafaq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3galtpfvr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fjefnqgg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rnlrykks.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vfdhshfe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrjqtuq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufmsdukk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zemxutvn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lpymokaj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulizxzgx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3omcvvjzd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mncodcyz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3msiyfkrg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uqplxuns.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kfzypqcs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pheadlhr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bvugcwrw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zusayzwp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kfsqedcd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yrgpykzn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqqxnmvx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zmzutpwm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ijbvaxbs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3olnaawda.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ajfowdxx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qaottczi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fytnzrwe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3almqkbsw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xiaqlvpb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvkgbu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3btbkazpm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uemgydjr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvlimxnb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mbfbbyeu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pccjinuf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywzcfydj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iawafahg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3grdcgchn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hahocwad.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emukxyft.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3telkuprj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3aiyemxux.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3igfeqgpk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cjuacpha.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3skbktxwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fhiqhdty.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdnorrb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lesuyodp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hnjhepin.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rmnzqhbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qshfzxyo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylrzmedt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrwbazf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dtrkceyd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cuklkgzj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cvgvurjq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xpmwqzik.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxgzeijf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pbkamoyk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jtaltbrj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3toogsigr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vawqvjca.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ghnqctmj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vhpahfgb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnimbjdt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pdypldpv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htzrflgr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nejvovfb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3przeandw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wqbrofmu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jrmqeuis.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cwemhhxg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dvticsth.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvcejxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcyxwyoe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3odtygecf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmkrfjhn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmavdgdm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fcpoobku.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ptzpuzkn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kzvrrzhm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmsafuib.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djtfsopo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3unqwdwip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qtkqhuak.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvyzdeug.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uwpzieun.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3newfgpoq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nbacqjuo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jotorthv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zjncwpad.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cbokgzze.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mmlfcsxd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mzpcgbds.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hmgamdse.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofezcrwk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mhwytapf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aknoltmx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cqmsohpk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ikorjqyo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jyuwjhkl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3otlmynti.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mbfigcep.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ogmtaklw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3htwtkfkq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xuslcaji.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsszibpl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3trbkryvl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qfgxszwi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rzlxzshs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ypypmqbk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcbtnnri.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tzskejpw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3abaalayz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ryehskdt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fsxwwyyf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tisguyai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tbhlmuow.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wxevuuix.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urlhyihs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dpdyosly.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hjbdrbtm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jdevbqws.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jjyxclec.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3srkmzcyi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3drdyziyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3raeukgjk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kebyvews.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lejzpyqn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3usybebmm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vhrwjdxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uqmdpwqd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lduzfbkl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmycqagh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slexqmxk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3racmyhzq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xqtouosf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3idrfkmed.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ibuwvcym.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uwzdocgw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pczajeue.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3whjezpgj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wvbbznen.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bctcnqfh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrbalbzr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3suqzlukf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3juvzgkrt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbedzi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3msswrsrm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbozzlvk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jbyhqfbw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3znpiltvw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ninfygoe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikipuwcq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xcqogpvv.html


<!-- 参考信息 -->