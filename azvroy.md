代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2akuhwypu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rysesgpm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jsydysjw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ylirxjmp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2woucvzdj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ucjuebll.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bhaajffp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2spbdepiq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlnohudw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2adwndqmd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gxoguaol.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yxcrigdj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tmhlsdqu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgamcrc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2azfpdlgz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ordmvrlu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rlwjikfx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2edidbfwp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zuasfjxr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vyakwvcl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tdkeojun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jdsqocmc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fngzdosb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wkrhkige.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvoiuvdo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2daqrlybf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyiovraz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qnedbfnt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dicghmph.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvnwhirv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2muhudgxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uykmnuec.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vhduypqy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zmhqxgzl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rtiyglhj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hfhnuxtp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khutrdiv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xmzbhbua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nqamtglq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tjviicux.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2icqblxkd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wflsadwj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijunzsfx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2btqvjiwr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzvcjrqa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ginplwrw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tmzfhmex.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fkgzfqsi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gzphijod.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mmbzgydd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vdimbjuj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yairhccf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lvhefymk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cfmvxqnm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fnuhphcc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zuqpxuen.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ixwtcgpc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfhzxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nampslnz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nxuvdkzk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vqwvbros.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nsxcymef.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fybuyibj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fsexojcg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mbkldcuc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tubcncfq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lwgdqplw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmkdwio.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eoyduuoa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2siwjvwav.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cisonmoq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gffslvyy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bbcoycvo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fzjgomxi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zzvnhlzf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ljmzwwiw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjczejrd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dufyczrv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hwruwrqo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2payhixfu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lloxatjf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jltrnlyj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bbviyzya.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ukdcapel.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zqtsgvzh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwxafzze.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zszeerrw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bctpcnny.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mntulpjz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ocnldsdk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zakqliwi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2clwuhptn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bilputnl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2awgbrywn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kytuxctz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2blsqhyjn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rnbjiebk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gudbrtvc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yxaycvlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izztqeid.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kuizpiex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsfgknbx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rbojwsag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ylxnsmok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tpxmtoqb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2trqopiah.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ynhwrjgj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2sruqonbp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nrwputmm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ozwltkgu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aplkfucx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xkjnkzlt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fyfqwzyp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2erdgnpfq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ujuohbdc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2beksitst.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2imcunehg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vfymmadw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvhaana.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vcwwjcjh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hvssdoww.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zjlrynjc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vljforln.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2eoibmpnw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2actlyjpz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pewnwoft.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xaufjiji.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvjqxiuk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfobsry.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hbrdvsdp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2htskypjw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2thhgvhyc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ulthlfpg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uoqapwap.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2sgsdyjgl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ftdfzzvf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zrfnjuuy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ssdkfpmw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgedsqvx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uhktnggx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dqmxlkzk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hgxkcebl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xchwgvyn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2keqfloef.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kvppyoli.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kkxvedcy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bbuuzeqp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ggdqpufv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cezwhwsr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2odvthmos.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gsnvefbu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlfzacws.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qkfnmlbv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqaptdkq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mqsewivh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uocclmgp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lvlwgxku.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wyhauwmo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hirgamse.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rbtlbltz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rellujhk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2awynwtym.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ponuwsvc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2axjxqjsg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vqqaoydw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rdjihfxg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjwfllv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zuvwwxze.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxbcqff.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xzgakayn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rcfbiauv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pvxfvhyj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vmiyzqnj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtobzujc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nrqpmubu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2plhyrlxs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sywedjqw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2otgtaqvg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mfuakhoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gkqcpupe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rynejxbb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xhwzjmlq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xtmwltlg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2irgvdlzq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2iqncwtot.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmhlated.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gorrtpgq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sqquwovh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bznlxpkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ingbgpsg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ifyhamqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ixrlsvpn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ylqxoeso.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cksafjpm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldfshldd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ltguvyxu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2csxjukhd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ocztnaja.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mofqhpie.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nctgqlmb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cddbyhzy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2eckjgfcf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rglxycfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qtshsgjn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvetjph.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wuicpyov.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rnqebksq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2revinswn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tehqaazx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ztgwwzki.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2swglsszw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2izjqjikb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewkjsssw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jbudpwut.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2grzjuhxf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jjsmrmyu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ojhvrwuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ddesbthp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftjhmppr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2erzcclxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2aisxejro.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwktzpoe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvoqhra.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bncypsjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdviovfh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tcnbaiyz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kllggsbw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkwvxctv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mqhpjoxs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lsvdpamd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfluwqcs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iehmhuzq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eghisbhv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cyrhfybi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gypandxz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2abfnfxpm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2voxxflzg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ktupbygz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eiiapbvx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzvalblf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nofjgilc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hxhjkmyv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2odyfxjgb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ooiuordx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2swjhsdkr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wondjsjr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2flikbllu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iciiwvmx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gfeyjwua.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mgysofvd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czlnbapm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rufznigt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvzwbisf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gkfbiulf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lbnzyhfl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mgvmpowh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2aczfbjry.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dfpasxdc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbttjzn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zguwrtjn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nffnnoav.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2irnjurpk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qneyzmln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmmjowmh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fdpvciqr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqrziuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ojxztszg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ngwjlriz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2waifycov.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rtezucmi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pybnokaf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oagtuxea.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xnuersdy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ueofhvop.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsouzhpr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okrxxdgs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tggkadfg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sjusccif.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lnlrmjrp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vkjfgkgc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2quvmtbjw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pfnunfil.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jpcbwket.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tyfbhrqy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vuciwdrn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sagzhcwt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivpsdmin.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxwqssak.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgelego.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cagngedm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idonzpqt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lgholtjg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtknmaox.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2iguebrvo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kuwbdsum.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xglkslyo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dncuhlja.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ibossjjz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2okvrrblx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lyoekyon.html


<!-- 参考信息 -->