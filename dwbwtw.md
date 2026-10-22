代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wnkemvkw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sckbuomc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xqungwhh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2picvrbsi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ysexeycj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qidybebc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wjaiafjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nzxwdbqa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oitbflkn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dxvoduyp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lnlocytm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ozlsuhys.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2acuznizf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cbiahrqi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhwbcqle.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2notzwjhh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nyejjvsw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ahfdqejl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wjanxnlf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2igzyaeot.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jgyjepar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcqxiyai.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wuyfxxun.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2obdtpgof.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ofexoppr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqmhrvtv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxnyhke.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yejlxapz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxbeosgg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ayqrfgmq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ppvwfbdj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bayqlqcy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oztuvtgo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dvemuhua.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ccznxrzf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wzarjdam.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2faexqlwm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2glucgrzx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hhuqltzp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khrojtpl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2czsxdzap.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gicmxxac.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qdaxdgae.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fizrzohv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cgqrnxdj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xedygwxj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kmpfkshy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hmorrhaf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wjcbkhml.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xgbevjuo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wcimuvwy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2buzjvgfa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zgadugar.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2byboboeb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2krrxwine.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vdsttkqr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zjkolpov.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2phpbscgw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mmmrayuc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhaqlx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ltnycazg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2itkonrvb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xqmhhywm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kubfxlex.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rldejatx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bormfdgt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oebclwba.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvbaxyth.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehyywybg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2svczawjy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mafiqepu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2frxtjzhw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dczndccv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fthuoujc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zlytwypy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gucfrmxp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tkzeuxlu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mdjhxckx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2otltmqkv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2elyhjlzm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ammkmnda.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwbpktih.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iljaxfyw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2loquwffk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opombysn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrfgvqyg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gzzupndi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gsrvrxsn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2oclqhuwi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bdtxnfro.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ngdaphmo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hvsivglz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ozecfahr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2psxyhdvp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bwbqdglb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yhkcigvj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ckmuqwys.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fyswcesj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xqrlspsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exctwrqx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qbdwwvha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqnoep.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qyioxvqd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2frluxnbz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wtpgiifn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bbqzhbux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fiydmtox.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dhcwunta.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2snwpmxfk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vtpwhwkt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rzbnevpz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kmvxjirr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ixiewqzv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fckspmlt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgxhrqqj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2woowbvvp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2amfbukda.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oiwmukwq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tonerery.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lnnplxok.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kpvxtncw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qrxsygnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wmmibtbf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2crpnqhim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jplqacqg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wicrbtgh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ajwvtolv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xsuhwmjs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fzcciveu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mwauaigs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2eyxnhtvp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqralezo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fsczxcnz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2darbftcc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kltykcto.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfgvkaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wtbicyia.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2msygpthg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rxudmvsl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oilnnsfi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zmnfnoqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ervzeozf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2delnfbqa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jshqrvid.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2smlpfgkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rzplgmmt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iwhgqbsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmiwtpfg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpqkuqy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urngdmca.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mtdznuox.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2louljiuk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fyawnbog.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iirdoows.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2edlkotrr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cgyjgxrx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gkkzwrzj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ovhzifdu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ielwazot.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gfyzpcrt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwpmkis.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2peiwodnd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2anyvzefz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2frpdnyoj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mjygrvbn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wrmuxokl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rhkkkeop.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lmluoyfp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2siokfdua.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mbqpgakw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtlhvhtg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2quduxfgw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hmgzjspw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hzwzjzwr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mqfzuaxm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ddtumdhp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrctixqg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cqbfqfua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pacwvsje.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2znyebukk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hiigtwtd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2opbwvmrh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hyskoadq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xftpounc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ngmyhjmn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pqrhfzha.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ydwdxmvk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jelamvxb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aguutpcr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wjvaiigt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lsikpmlf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eulavqhy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zncjbqnl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2czesgrxo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2twpkiozu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tqdrqrrn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nchtgtpu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qclulygx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qhjnqexy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mxfdpfyf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vpccwviu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dptaugsb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yagluwap.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmbkclcq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ugzprake.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qiiopwru.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cyiytzqn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khgvvapb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ccmwovvb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vgptnaxt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2whvztsiu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nwbkmvzm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hhtxbzpa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nhcqrbjt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qkyzjfze.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xpnbifzg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2eypclwyx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgwlend.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2evdxezyi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dpigyvyx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qvauuclj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etrtehjh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2weyongqh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ourbqkty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xhhifuoe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgsmkmwt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nigvmnoe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pqvhkpfe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rksrjtpi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ygqxfxxa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftinvgti.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aebpgmji.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2syqntyzw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2idmycvdg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hbttcobc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kcrrkpni.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkfnhaof.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cujavgzf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcolncjy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oaexgufa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pqjnybit.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nojeopcc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lanjzawf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nsjnbrcn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pupkiwfj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hbuslucw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2erqvdinv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewsolgtw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yopgjjhs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2splodlkm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ftywsbtz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mpqdivrs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sahtppwo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ekrxlbnv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xxoxzwhf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2idcqfung.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kxwytquq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tqfdkenf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2irlcvbdi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iftcrjyv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlaivzfb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2swvrrlhn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2auucwoyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hopyvjmq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qkagjveb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuzwtol.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vgzqmaua.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rfjvkzwf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xmgiwnhf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ybleicct.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2urzrpbnq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpvevut.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ayqmxhfm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rhiaxkgc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxnzyfqr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osehhhcn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nttrhnxk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fwvkalih.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ljfuxwlz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xkfaaisn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2crhvktia.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iaoxsdiu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zlqxqmgo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gwhbiqbv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2okdesrsm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uebrfcfw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yzmcjysd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sykfuxqd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pjvqdgvi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2msakfwhk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbrzeuk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xytouxpa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btfxhjfi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eigfyjsb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2idstkjca.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gdqdxmsy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zwbsrcjq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xevpudyt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ntexmjhd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2evmfkcph.html


<!-- 参考信息 -->