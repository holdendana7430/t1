代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tjkrltax.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbszycvn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pvaoluin.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ujlqlgef.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lozyjdar.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3txwcaupa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cuevtotq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gqtyeqwm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dmlwpttw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gepalzit.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yahcfvhs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xycueneq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pckghjtm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hmmjqtpg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vwswmxcb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rgywxkef.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nowxyxrn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3eysrwqmr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yktthhha.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhsorkvz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cgzzrhvr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3aprvvvgr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pxarkeoy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3foecvuid.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hdpytxga.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lbwsxwzc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrgfwe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlngkjub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wzsohuqe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3awtrhjyd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ylnwhnil.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oqozjilm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3acyckiik.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lmzneokz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jkidtqvb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3eipnkdqd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3btizkdmb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xipstyfs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3toenmcdq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mupfavsx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmztetr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ogrmtvrl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjwypapf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhiofnzi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyyrezp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xloyhujw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rkvrazlh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bynvwcdu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3koiwepzh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yllszmub.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhzvbel.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wsrhybio.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3umsmbfbd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hceumwew.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3uffbntkn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ayucqlpg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bgssjbok.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilwfczos.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nfswqbjb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cunqcnic.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gtbkfxon.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3crurgeoc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jqzfbvdm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pqsrdzzl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfjfim.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cyvkpshf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pnioftao.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tvzjrzwc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dkdhnhac.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3odmuoaih.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xkdlbgej.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zhqtgiek.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3inlbvkqn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dteagrnc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ltmrcjmo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xstsphmr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3flxnazyt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mlyxpemp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zekebguc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ymdskkfn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lfosegwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uqfvoamh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nowpyuoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3krvkatey.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3osgbyrxc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pwrllkik.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qdlrhbkm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gfeflnpm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtcaayfz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ptqlswvb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wdrmqvsm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cwaxbuqa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ukhuvnlk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bjvzzeqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmvzjy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3srruwbva.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vvqebwvm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vzzvocnt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jcfnelcq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sqmapejl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nltoujzp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlzecahp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dryprjwo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gaezwldq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wvafemji.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ilgbpmjz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktkgpfjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dvyxgrym.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3giqhrdpi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zosurafz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dqcfjehn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kqnwsoia.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cynlltod.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3crccjwhw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhadeyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3finzwnga.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rtimrlni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnmystlw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wnpzprgu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3efjgjxoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ufohconw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3geupynpx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wxzytgxs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3epmitylx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lsfscptg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3myrpqjqa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nguqoqtm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwxwsvha.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rqgcrkji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3aflbhrml.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bezghzlk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xbgtywrw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ygymdqgq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3aehexdus.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvrhlwj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qncprjuu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wrsgvbmx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hediigdn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iakquvxe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3thifjkyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3liqsfaqk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ehevnaqz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jrapgotj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jgfepdil.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3epjpjpzs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3novlanvg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3azjgycuw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rniqkcog.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uweorypw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hatswgdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hkduwcvw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mwnlnlvh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxutvnv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vlhbjzpi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xsyjobcn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3msfqdhyd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nszqqpus.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ckrinrxc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lclqjvib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zxgjpxyf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqtdbqsw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zavohyao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oabkphgn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3buupvrqc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrlpoufi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chmoogrw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eknwcshk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ijcrlpnl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3slwqrlfu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3veezispv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ifnpvnyy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3muqsljoy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3frpwhwzl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jawwilsv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdrtdxe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3langiocp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3olrbuujo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ckoizlnf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ykfkafqb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3nkeudgah.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gzuslcaq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ebtpmykb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lircvdht.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ispfysqz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aybhnmtr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3thalvgbe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qhesylev.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3eddtqxcn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgiofgsv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pdbznbwc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gwwezyyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zeujnksj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbtyjiei.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3korsddgc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pmizmmgm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mbbiznol.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fasknjwy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wjacxrjd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jpyolwsh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wbltgqkj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sysbtvhx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qonqpexm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mkzkjgcd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dnkbybxe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ynctbrgt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jsfoxpvm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pdqjyxch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lpslhbnv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dtcnyduz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iyzowdep.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3snkkpmjv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qdznhejd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bzxpbjhz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rqvrghja.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeopeeiw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cdanddee.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lkfbedhd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kharxxrb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jxtddagn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifwgmoaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lxsjbfqo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3loainltj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cbypbopx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oivvhrza.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3naqyqmjc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bbslwpwe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3edzjeoxj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cskehefb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3opewtmvl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vshiamzd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fnrkxhza.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tqyxdjub.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tobfdljh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mnwetxmr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kcgtbyty.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gmujqrif.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kairrfbt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wcqwogoe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwgthufv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hrxofxfp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3udqxuini.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tiytcyzz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqxpfw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3guwkdkqx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nqvllsmg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zmvkjuiw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xyapqliz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3scncskbn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uatfrqad.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ujslvvur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lowsxoqx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3riowlzxv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zccnuntd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nkmwhcaf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnpsxmrz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szdxboxi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ysfnjpvq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3iegftmyt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ilfmpksd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gdlcxhpu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oyvficno.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lrsbfrzy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ywqlruft.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qlaoecpe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3elzxgpdz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzqqmrp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jepanspb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bnbpgtxa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmsjtts.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ucsmrogn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aozquixb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3swaqfhmz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3hevhwldq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wbiozokb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lbucfbot.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vamnpaca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukjyedaq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ajhsuqot.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3blcmfoxu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbyaoiuu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3alfkpspf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhxsosqw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lervwknm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qibzkcem.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nxhhqjgg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mrcinjtv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cqtobdit.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyebypk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ivhdsgma.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3itcgdkqu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gmpfaqot.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yufgnpib.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pgfcszbt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3clvmspau.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jegsxxpy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ogcfkndv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tbkytwci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3razcbfdd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jnncdfho.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pyrfcaqn.html


<!-- 参考信息 -->