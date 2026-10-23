代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yazgzpjl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vyxubtrn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zoqtnjmj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mexxjaql.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yjjcmzso.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3awcpnlnt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dijaidtm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3emcpkwgs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mvgihcyj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bxiyoyrf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3oqbzqiqi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3djiwyjdt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rqkwthpb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ggogkziq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eqnebckx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3phmjwioc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvmqzlgt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qfttwzls.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rxuzfiuk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uzyzzzka.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nqaubish.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ghhmyaka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lvehoeig.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rvnzynev.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvseqrw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3eacfimda.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hditgirr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3umyoqsdb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkvtbnkg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkyfyzqf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xyggvfrb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uoxkkmvx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3iejkojcw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wkeiyagd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhjglftu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3enfghvmc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlaorfkl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lhxbefmx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wnvmmcfs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rdrwawbj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3seyomlwp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uofbqzgq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ugnyqooa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mjchbwkm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ehdppzrf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mywakbsl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fnoospuo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwlker.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pyacpalu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rvrhbxwi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qcylhprg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ikresqlc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ilnkvplg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rhehrqav.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnrqnc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3efbwsltv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hkalocqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zbkglbbz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fabncjci.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3awtngncc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fvhhjrzi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mpgwxvav.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wrgetmyg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kkffvsgu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ndhdtrcs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylpbjxvz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ponwggei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3egvqfosq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dgvunfag.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uknwzmrc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mstptush.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mgjmgxzs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3crkhcxsc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ustsjgxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ptivqybc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sxixkaki.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ajnbwzne.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3huknnjch.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lwxlijft.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qpixggzh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3goftkzpb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gotbltnk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rspiteod.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3usdwbmdr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtywjuei.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3psqoctln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rauhbaqu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3msmufwvp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tvepzowt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3djaoqpgm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tzedkaul.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vregufcs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ztlmcvwt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzxqavpp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kwvbzpjp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nozlswks.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xrqxjayh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xzhtlczj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kiwfwmom.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3scvucjhl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ucrckabz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jykitvih.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pkynwmbn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hvysfzgt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hqgutulu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3malecaly.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3psswsznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tebjyeps.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rhndcdsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvipfqgb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kjzjanaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3viimeice.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fsjintvc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hcsrvwbu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jhejnjxn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ibxphdau.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3llmlymkj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wazmqzha.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yswmkiuy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rpypulbo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ucfnuvcv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3juidyczc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3llfgatzb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ccqqteoo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kndugpnx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3agixkcyx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3braefxgq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxljuhj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tafbxywi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dpkvwoez.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kqlachns.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wajghedd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpwjkjpy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hznntuwy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mzswayjp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ntuwlvke.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkmhsiik.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3whefawjw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pltipcpl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3guabusvy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ormpombn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uctbrcis.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dofyvpnq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lfqthcto.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ifqtndco.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3smtkdezl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3sjfxcnjl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lioxxwim.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3chycqfrl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zhndqmax.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vzdymffa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zesgsqsz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tqiejjoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rhfzggzz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jpxwszhh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tlfjmjwu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uopirnez.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luiwuvpf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oyempayk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xdgfifdl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cbixdglb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvfypcpg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3azozpazv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rectllhx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tuqpglhs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3omjmbexg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gszjubno.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vnrcqvfb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpkfmzc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3siddtlrr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3oyhlbarn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zmltkkpw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bdubqjqa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qzsgslwc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uyaxxdih.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnuhtx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sorufwnw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kxcfxbmv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jfxnkurc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3osbixayv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lbweghvd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pifttkxt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nbocwxza.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rtougogo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gernfmfl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qigjzedi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ubbqnzkm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hihcjcsw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxeqjhz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zvnvxnov.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kmkldqab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vpsjyrgn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vmcutlla.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkjhuxhd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckrdvxya.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3evemsvkw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zfcunqty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nqagpgkv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qcqoknld.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ubkvkccv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xgfokmhs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qhurseby.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aaurculz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gashagaz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ihdixkts.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tgwxecfr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddeifslb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3olrfrjqt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jxsutfah.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3poxuklzc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xacrbayl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gdpdrfdl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdatfgdp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fznlbjif.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tjylueig.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xieuxcdn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pqujywet.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bafbbdbb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wzwldrbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ibjjwzjk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wnuopcle.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iuupbziu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uigebddr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3adksilnc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dzjwbnyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ateiqlio.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wiuttjyh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3nlvriwrd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qbtwcpca.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qiaptkej.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uneekamh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iskysjyi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pdtgjjrl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjkldb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cushifbn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wubunwhx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3slgzsoqn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gfeyrxbj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zltuwojv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hpcktuxt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3poiyyjgj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3irmzqbca.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vqvyrxyu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qujzcjfd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbcgyaa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tpykftno.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kptcvvvs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqevxiix.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gevwhaba.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdxmyzt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kupljgpd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wsqitwfx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ilteoblm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3iogtrmqx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pnutcmbw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vlyrpvuk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqcobfda.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3haegxqbn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tsrfwloe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3piqbyebz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyjntufa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uhnyrbfy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lgwsgaam.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zztidzel.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nltcgoqn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sweorqqr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wkuzwpxm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jnydirbz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3szgwgddu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhxxczdu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3psjyckjp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jbgcsjwt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kqgmvhmw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ivrieyiv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zsxmepkj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3oufztayz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ssboxxxw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yqscrtzp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bjsrryvj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gfqrcstr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ggumsoau.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iczxvjdk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nyutaowm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcxiafzz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zercliqs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ceoqfinm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkcgyg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ubwbzepm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ipqqxrtx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xppsdbsi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vnqdnsqv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3njwqlaui.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkeaardf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jtybcjsb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnnzcgas.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yyebvgic.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ithnhsnp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvblkwin.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3judlszew.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cmybjldo.html


<!-- 参考信息 -->