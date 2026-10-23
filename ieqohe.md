代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uobuofsj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ewulxnyj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xwxrvtfj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hbndokmt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qhyvuqxf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tpgiyewk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fxzmglad.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eerjosih.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fyjliann.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vdlzmifp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jxfflwcj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vovuebty.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xdurercr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dmcqkphu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nkpthavl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bpdmbiwm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gcclqaas.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uhxzborh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bbycbbne.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3osjgojya.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqgqqvk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ljuehngn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3npwyhdtl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dimaeikp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3duoedopk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3njpnqync.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxelembh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lhzusqtx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3frjybglq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzpupbsg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gcixejyv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bxdcbqob.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qxilgwra.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhqbycd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jtfecqvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3anfluivb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3estqegtw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3grqqeush.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ooqrgzbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3veovoxvv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hffmrmrg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wcauzera.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kmpviacd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jnvgvwmw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iyjsulow.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3udtsiyjg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kmqapdhn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gzaogxcb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pbylkwxj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3afrtferl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nzoeyvti.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wqrkwmwp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wdfttecg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fdghjarw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ezbufpbb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3aonqcjby.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wexjuery.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qnesfbqm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ktlxfhvj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3sbgizbuf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ygposilz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bdztnqvv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3slrpcsmz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vswobqbs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3habasoyj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fewsidty.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3npvcgjii.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mxntqjvj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3chfzbbxa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaswezmn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3loxjbrso.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ioburiei.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsbbjbpd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vqdxcbyq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wapkdkbp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tjkjtwcn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ruhjvdin.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yjeovocr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3upxfujtn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ogbbgjhz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvnaxey.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkumatwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jgyjbwab.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3maupvcmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3brkodbhe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mylechfd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lrtvydlu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ddhmfjex.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdrtisbi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3oqtiochh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gyptbfup.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jwtewwba.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3scbmdbdq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tbqfxpku.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3degvcyyv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3naholzdt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zoqqmisb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3reoepfhe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jvmqqpnz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bvzahxsk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gjuoieuo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kfmzabre.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymotjljo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3laqzezvr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3aowftnrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzvblcuh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qyfwjjse.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wosrezet.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fmbphlry.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtaogc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fgexwjnl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3yimsxoce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sjqzjvxt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zsmxujtf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3suniltkn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hacgeiti.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vxgbnwpa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kxqkghse.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhkmnign.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3biemjayu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3enlbwxfi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gyugqoqe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vumiftap.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3clxlsuvm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wslfkuoj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zusqpknx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ytuzvoxt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mqaflcwb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3roguzafl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3usdkkrib.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ickhamrm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qjodmcgm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kuqgxxzx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vewqmxpq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ytbipnge.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gvyrqeem.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cxvaijek.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgwepif.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbklibyx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dugcqgxu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkpyvpes.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wckbtfia.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ckkqgafa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3voysjdpn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qzsexvvu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uwlrgdwi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hwnposuu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tptxszmh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xfeblahc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uzeqrlam.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fbfebest.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jpcnvyqh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwiqgtw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtpbssxe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3axyjprzr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kpkpfqvy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3smdhyobd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwvncff.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jdcktbwx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hwbphmmo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3dccbvdoi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rfychish.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pmwwtyft.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3itjegbbo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3grjukgzz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lqbptome.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zafcfbrf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3glukqpac.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubpuqjdf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3riendwbj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3onsbbtxz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxsycie.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xcuvnzpt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lzcpffcv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yumjqkzw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wkjtutkj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ipsaptev.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sgfzmcrl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bvvobkyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kpkhixts.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlleztku.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rwgmuawg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3buekhood.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yzcmdclc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkwvqom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3asqxajih.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3htcvzwxt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iwpqbgwh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gshbmefb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ofnwjfrt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cswykple.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ercurrcw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jvmfioed.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zyqqokbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nhjbovvl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rfsubxlx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3owkccpvc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wcsrrpwv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvnagaw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3deapjqqx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ymsdclkh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ohpyulod.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqieftfh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rnbnlimw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3stcfrahn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cknbihxm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3sagvonae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cigoupgx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxwmcsyw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dtviyszc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bsnuzppe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xwewdbjy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljoyvuqx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ielwolib.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bqfhxret.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wbfphfec.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nknzrkgy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwzxvdr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vehcwpqq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpjieuub.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aakxpjne.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lkwdrmje.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zzyxjyos.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mhotulfr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ddmdjkmo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lhvtpden.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drzgwkhg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nklqkcpp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jaaossny.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bfjmpbaq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qssptsyp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xemhsqty.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qsuatrrg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dvnrnpto.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3roeahtjx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xizwaoie.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gbenwjqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dlcrmiug.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tjbehrgn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fqepvwfu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uimhrzbj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tfszpdcn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkcmaxge.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbqrfgiu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zngumpud.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xlesqycn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cdnjfslr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kgxtrbhp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rrjrcguj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dbkzenoq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3fexyhopb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlauutp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbllgsxx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zevawfye.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3btlvgpoc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sbepkzsn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxrweju.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yzanpqrl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xeshllmj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ztffopul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rwdzlsnh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wcyrjuut.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvxpiz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yspxkyku.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvyxudyw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfoeqojl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kdrqfcmq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3daihunjj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ozuwgmuz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kwypaqmk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vulxdiim.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iyfpywzu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjqpvgx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ihmnorev.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wdqnrhce.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3izrgpurr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pkcpyfbp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aiuakdln.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eihzbfkw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hflxoqcr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3anwadomw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tzhcxfuq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bamynjcb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cizlllrg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zlvanboo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3algiadaf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnrhvohg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dalepywq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3skufpqnr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdcuccex.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3orsbczby.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3idybkqed.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfvstxh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nrktrrms.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mbpadhdw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kdborxdw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnvxgdsc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wmpipcwx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiiiyitn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vcaltxua.html


<!-- 参考信息 -->