代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hajhiygr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uxpvkzzs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jhhufshb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrewejt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ihytvnvf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2urtgigls.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kbfomtqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jvjvpqhh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fmsiexkz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kuyqlfew.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2sgcvobyc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fbzdpkbu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qryvndmn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kpltpcvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2azdjyktt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mxeuywnm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2phssglna.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vuhskult.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cedtblbs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mwaflmpy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2iruezioy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2eepdverj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2loxwwggm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wiortqev.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2enrhoxrg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uzraowev.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lcurwcwz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2izcobfdw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycydapit.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmprpqoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsqhrdu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xdtbjhot.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbwkhtau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mxdqmord.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkioch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xlxovxzh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zmpkzrgs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dqahyuuk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ghdrjkjk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2apphjwst.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2inpobvcx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vkbrbbcb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lsdzakge.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bvvwimsv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rfhtwlyv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gozdmweb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdozvu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2itvodzvo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mhwgwrgi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wktahrud.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yelqqocy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2albbebgb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wdpeqwhl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uqoyhiuf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rufnqrbc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2woqgfxfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2quzxsduk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tokibtua.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsqthjba.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hwkqmpff.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gtcdocij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2saeluwmw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cjfqksay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcmeedzg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tpbvuqic.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fvxqwsju.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2afbshbib.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cttltwhc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngpcspao.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qmaqypmy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ixaabtoz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2swmjutyf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qaacnvoy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcwqtovo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rvyjajfm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dvwxxxsb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kyrjsfcd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xtdkjcub.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mgdpcssc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2avdauipo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vycrxryw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaluuzrs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2elmgvxlj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mibqaalx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nkqldlio.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jiqrhzhk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gvkbokbb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2twfmkxur.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gyppcbvi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qgnipmsi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cdnacbkl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xygfrmru.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rpmsoltd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fxigaiyw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zcmykgus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oscwhtzd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wepjrveg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zigukzbi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jakqnhjo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2efmfjdbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gwvlqpgm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xrnkaubp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uegfrawk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vfojyqkw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mevfyhkk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2amzjshgj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cmkddtag.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zzxkxmvk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fhwtohzx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2soxfmqlq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dlthehdk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kkwmdzsk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jeiizeth.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lamcguya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjzvypi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gxcigyes.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2faiolmon.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2brpdysfx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cnyldyph.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nvvyffgu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jkickrty.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2frbnxpev.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uumwpmex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjbbtgs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wpyxfxye.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2etgnvgmp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtekfhgv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngkslcfx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ecxnsbqe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sfmsbhes.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tapqnoff.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2crdwrjev.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gbvvxpns.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cspvtnlp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lfstnbet.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ufwahyru.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2acjhjyup.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oauahocm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fyiagmdp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2aajawjkd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hvaycoii.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qvvzdsmt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dgwvweax.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fnyxqkrp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aefomkej.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlpzfztf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oxjnlskt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2peuqsmxk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bxgvgzqe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oesqnhou.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mabdsmwh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rjiyacof.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fmpvllki.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sgddqytw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zbuqbzsb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uizqvzhm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ffgkrwkg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aftdutfx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ytwoqelq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gohgfwnt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fxvtvzss.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tgdvqcyc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2swcdpmfk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nvzszubv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bocawqze.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2pdvoknlg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tijkhuta.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2egcxrsaz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bziwnvup.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tozajlkf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bgwaligd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qzszwnwt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nvjrmlrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2atesavtp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vdkkpywd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kzcakzjt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jallouel.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wtpucblj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2owgitoqn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xledhphs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkgdajt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oepqtocd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dlzowpqn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nykheqzb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zmxyxvdq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2iuwbujmc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dzermnzd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mwdsaufl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pnqmetbi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rddzmvhi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnfoavhz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pqnrqlwg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vtgjwlvm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vovdylih.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcthmof.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gxewrpji.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nfyfvhyj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qyuyoxuw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2spiizdyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nwxtoqke.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fltekyfr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dbmzdack.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jdxpmkzp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnirmto.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yadihiya.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xezqlcge.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hyslujvm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ugmvapke.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ussbqprk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzkywpbi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dcvpbnnb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtsrmvzt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2paqdpbdl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zcxtgysd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zryvjnsy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qwyicvvq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldiaysvw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joeyqkua.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lycavmxn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2waqtabjy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2whwxwgmz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zxqwkwgt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rvablhrs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jltnylhh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ejapvueo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcqrcewu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmwbedbn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ogojtzbw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nmrhfwey.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gdsykkaw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gurrywce.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2oxlaqfdc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bsgejflp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2deckrkni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cclfnfno.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjgscyo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wsdemwgx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ktopnyeb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2eknbhqkj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yzdgkwsk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2syeqbrti.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tyqoyclh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yafwmoro.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kurpvmgp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjuiosrj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xqlewoal.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bnbjcsuu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zgfthslz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfkqrzfh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aiwfpbfx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zsibakpv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xnzxhatb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qyxeslmr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2onhzaiwt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hpefrknd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xbwhtxac.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bcmcnyyq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vbqqzwsj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tbjujaxa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkunuzkf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qalkupwm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2csikobld.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fltnjyxy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bixatahm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2otgiwhnl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2grqfrqgr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oghhsmxa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eiumnyor.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2aluyyxga.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hozzkema.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkzaxibz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cvdglnlc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2miswqbhh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jumutfde.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hzhrexyu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rffllnpo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2khnrmgtn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2eaysumig.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2aodwsqjo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gkqmfzev.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nrlmomgq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvhttjn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vycxvjeb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkkcppf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpbugsmb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nwbuugti.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vavxokdn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bubvxgjt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uiakysgv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gnwqepud.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hnrxtxoe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jiqpspkx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pivbahjx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwljftp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fbrersnu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rzybugmq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jjqhgrwz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zzwsabuc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mmncwkld.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jlxvwwzr.html


<!-- 参考信息 -->