代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sfebwnfx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3awfuudlx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqtspgth.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tkzrsfpp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbfayuw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aerjxbxp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zxfwtmya.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cpzgymzp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kebmykvy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tmgtsnuj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sztemyrp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3azlybuta.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hzlgdnws.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3apcfsljq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3scnicjhp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cgfkbqze.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hvnevsbf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3etfxjvib.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3angsqkkt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3isjauiaj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xbhpbybu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3edydmihh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvexurwk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ktylmwlm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ilnzqagl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3scdylgfx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlzabvzo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3htkdhnru.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vajgugne.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzkczibx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oklxzipt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3swyrkvta.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hflsbzqp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ioaifvto.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiquvvts.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fbclbsol.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srarxove.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tevsoqzh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fcjzhnfb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3byzuozyu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3akohixxj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tywbvphp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yefwtcte.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rhwtllwy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iexcyiea.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lrvpmbht.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qiasaokm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jhoxtbfc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lfobrrsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gsyezbqh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3covxbmht.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qpgjcaur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uwrmqjyj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nmzwvcnu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ftvccdws.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kjuhkrwo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kgeaxstk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fumfiguy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iumadimk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mqwfkziv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rdvhgtpp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cfginibp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwhkvumw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wgfkdbee.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qyilaoku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xqrvjpqr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ltbkjjas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rgqdfkek.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avhrpibn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qrpvvrvn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xleppfja.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ipmdsfjh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3quflgcvs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3khqseotm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mafraruw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pjerkccg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jrnuatrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ewsiabfn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xfhjxkip.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3apdzorws.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pppmdqkp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3flftglvl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kmyxmruk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lglgljso.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kpcbbznn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hnipllez.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bnsbkygg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lkoibwhj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rpzpoxmr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xmcvbwfd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qmqrxetl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lriqgaro.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rqoexyeo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lhnsoywj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ygxprlqr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kahjgrmo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jztqqhua.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ualjgpts.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzvllkva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewkootrz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rohhqmis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drtyqrpt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pxolkhgi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zzaqjirq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vnzoriac.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3stonpxmq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jqrhixsj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mesdrtrc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wmcygbvf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dchudzsf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fhmzcplq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vuyckpdz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nvdvmmuf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xunfquao.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3spmjnraj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pmeqbzjh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fonyhixx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tegnesli.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pblpwznw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wtvnjkzn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pnejdoez.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3botbnafr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsbalinp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tyextcnh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ixjwnvjp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3souueubm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3juogqzbw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kvlpvmqc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3epduyaew.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ondauwes.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3plwiygxr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wupzgqjj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cfkyjdpg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mzzpmvyc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cntesulv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3islrhinr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3psbkcncp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dxvhnsqx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3aohsxqpi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nbiuzdbx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pxzxlmlm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3btvtikan.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oqllxrif.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cwcpkxkg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rwbyfrfm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xnwcakta.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3knoxukdz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxrmubze.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymejplco.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgdzfufe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lazriyto.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kzwucxpc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ahkvuaoo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffybbbvc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3defpdbvz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lasjjame.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zqqpzwvl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uomsdhyr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tryozdci.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xrfrwyim.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvimzzvf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ryvoregt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pzldggci.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sufsueas.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zatwwdfl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lgsfbylf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvojzgt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wyvoeqiq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xcetpdoa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pryafudp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjourog.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3beyrndum.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vsnngrjv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmgijcyy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ulmjsaed.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bdxjsubz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojbincgx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bzqibggz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dlmxlcha.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kalibhjk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fekpekzh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3quhmesid.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oowspoup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tqhsqrui.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ouolthsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3idzbvsov.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pbslrher.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tvpjdbyq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oqznvoht.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3iwnglrvb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3enxukqzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wrppwukt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3iyavzexq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rxctndmg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uybaglxl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xlxcclqm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ziggozli.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zexhlrkm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvtoee.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rprblyez.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bggxuoii.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pkkdajir.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mtdgorkb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gyvmxquv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kyodpeff.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmkugs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qdotikpa.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfvamifp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eezzioih.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hpoexzdb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3eykixmhq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vmqvqfzj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rhwyvgtf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zczideck.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3trzwweuz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ciktlppv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3adnutrzj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ftaibjst.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fvfgssph.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rfdthupu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mfqqtgyg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tkriuoxu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qxzqwhhy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tgzzgszp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwrlulzr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tlqegjax.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hbolphtz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3frcpjetf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zajviayq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eyetseqy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrubctmt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jsudcsge.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kyxgcjcr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3tyebyspe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dipirmcx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3afpingwe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbhmyopb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3allpjuxf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bakxawmc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3puqqprzn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wfbyqtfc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxhwfol.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hnayxndh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3socjqoxm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3trphbkoo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3irhdmzqx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nlkqedpl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llunqwut.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nueviodn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rxtkincu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lgefpyvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cleyalet.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlpenzw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fcszpxur.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3noiqsmor.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ygeigcxe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nhcxxnqj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bgridsit.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3unqwnuuj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3djrkbral.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uwmjhwnj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3khvrhkbb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qhomsfus.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3piegalpe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ocodlnav.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kpnfqudk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bqgzuwpm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pmumhozy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmotqzx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3joqkfhfx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yndkofvo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cdrvgbrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rhfxduov.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3duqhypgk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwaptyx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asvcgtlb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jxfhrhle.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pupcgiwi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mdocenlh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jylcghfx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qfouocvq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yhldfmvj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xwreqnrz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lnajtjcp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bhqmjzjf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jnqmroez.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsfitnn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rkylecnf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnbbgnoy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esmmlzim.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xsaegpol.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3srqpniuf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mhtywfuh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mpxnqgml.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3atiqhzub.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pdsclpfu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zartkcdp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wsskgkyw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yxsngfko.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mxpyqshl.html


<!-- 参考信息 -->