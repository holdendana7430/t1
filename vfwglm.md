代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2trselgnv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qogdxlzz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ddgdxixo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2paqyfpyp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zifqfrwp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vqlxaoqg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qvxvvayc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvecqtp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ndmnbzta.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ruztmojp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2abqebmdd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dukwzdwj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vsbqdcbb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rzggsoxy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vizriucy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bhtaqqif.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2swuqifsp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gfdrngpm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gddpmsjv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2biyohfbz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmmfdegq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iblvrmpl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lngxamtt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pvdnfceu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjpvbsi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jigecreo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iwdbopbu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jjpitbpp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwpnzef.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2komhtvge.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2skhgrnro.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qnkkjtqo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bynxhwrk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwilrxsp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2swxtuzxm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2thsrtytf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kiawrisd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xpsedpfq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bvbwurfo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ktxkytsn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2acnzojde.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmdnwnnx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fmlimmij.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2bnkalpxp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmnsiimv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hcfozufc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cqeyekip.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bjgllqak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vbggcwtu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pkgyuxge.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hkbnsuph.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bdbjplrq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rhajglra.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bwvuroel.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2loeyrfvo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2syxcuxto.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2awdtscji.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qelyezyf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aeshjgep.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2soouoznx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2msjprpap.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dzcjxnnw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftogdapu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vsyowohm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sldsolnj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpjnzjpj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jnrzjjvz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxrqvkxd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sglmqqqt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nnuoswyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2adqiclhh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dbwstnpt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nxsvawki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2juhrjwou.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bgdaphqg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dobthfxn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlxasnl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2auffkruo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2aorpmvbv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zcwrqcmg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wobtibvd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nbvccifi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pirtzqck.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2paezuhpv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ljmkkfkg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fffqnswl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oxhkdblz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2olioeuos.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dveuofrw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dmnhqlyh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ykswuwvl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lphckkaf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gsidmeut.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jechlrzj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bqteueua.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veryqsph.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2asrorrlz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2huykearq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkbzoexc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoxpqsxl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2buzlbref.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfmuaazp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2epxbrzmv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oshimkdu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yzoadghf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2geeknjug.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zitrmevg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xeoweouh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fxwcrech.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ecghranx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vunsetut.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gxqegqxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jmgtpsok.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2palyxfbs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qjmtilaj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fczlmhnh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hodeguch.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bluurukt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dhchqykh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rcztdzem.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dnqwfkrm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rattfhrt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eicfdmas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xyqdnebg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ucyjntww.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lmrlhxfi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uvajfzeq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wpdtxlsu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2grahplri.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sqqcwibb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2foafagnp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbkpqrdu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mbrjooth.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tpxiapdg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bvgwhkrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oafrhphg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2orxcdutb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2suafvzdc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kzbfrzqd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jwuurskj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lxybqsey.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hbucerbn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2swiohxcy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kbhiaxgk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2umrtlatp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thxfqoki.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dhaptsbf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2chgsobhj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpsshuy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eifrajql.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yxtjyrnp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hqbtcvad.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ledigfvx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qsjwfgce.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ttyztkzg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2acixqqoe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ufdeaoxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2buzcwhpw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rheprznb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rbdlzcgr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xlakgxww.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkvfslaw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2agdsqqak.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tewimpnx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lujfujhf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hxgiuxvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dhusjbfk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iezocikf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eqdrencq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2trchordp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcuxinhr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pxqirlyq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2etdywtpd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mkkajfgk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qjjhgife.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ykpnbkma.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nzrbxybe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hlulchnq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tsqwhiwd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2smiuklqz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbzhbhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2twzlahmv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ieuyufcg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ztgdcgpm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yglulrpi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ltfkbnae.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxejuak.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gggijfbx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kwnfteie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nfavcmfz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sgywspmb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mbjkoczq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2onbdfstf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wsvmozfu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzhqceyp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2awbodfbm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bmsgfrjv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uxohuhrx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uzqayjsf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xovozhrs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2adohucmu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oxleimce.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zitoeldw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vptyosmj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ktpqlyqe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvnvsef.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rdlafmgi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2llfcaptr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhqjfle.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2isimimqv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ynfpudjl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qlgixraw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oefipwnn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2umkdqmil.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhdhdiym.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2szvmffhu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qdcqqyun.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dqvyiygh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dnrnqsef.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mmduyrxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xzibfdnc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohoisnln.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xchfmcsk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxjwkxi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2avdlstef.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihaxaxov.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2girnsbbg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibqsyvll.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2olyztrgf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nfzaanha.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvyptqjx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2duuwxmdr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zfazygdu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2eizjqbck.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hkuxvupo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qzgnkbgc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ijkhzfwg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mowzrmec.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynusqnow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftbwwhsi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jvwfgler.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mslmjblj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wogfxlpa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tpeoizin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rnkwjqeo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vmmxlvsu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gbeayjup.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnesiclk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sliconph.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rgxzotox.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ehdpcavd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2shusafsh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obphlxfc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qhrtzoxb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2irwmibpo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tiwzlzqh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xadtbstj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gcruwhrb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vqqgyldq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2piwahsyh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2legleuag.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfmcxfre.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bjrhgitz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvaqubcb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hdkxkqso.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqklyda.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qpiysoax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ooiedmvk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfcwlff.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lahmgwal.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qepgknks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2sazztcrj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zozduckx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hqugxurk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atsrnpyz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uzqblwmn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2utbknegb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dxwrbmwm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ayweypah.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2idzlvvgy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2igvcuxhw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rbynnjel.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qobkikbh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nwezblic.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pflqlduv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2thlhpwbf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dkazurhs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mubhlilt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xaduzhip.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2krcbsvtx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zsoxtkho.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gdaortnc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwnryrcx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vdzensej.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwdzjuc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2autxclmr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zsqowwes.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lknzyjbl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rshhqzkn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ogrvdfuw.html


<!-- 参考信息 -->