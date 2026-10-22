代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2utcjluie.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dfvqqlzr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wrvyeyis.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vqlzwjff.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sdhphtwy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlzhfzs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iracxjaa.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2odwkiauy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2amghvqcw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mdbeicsf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wzytmsdu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uhngtqus.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2velzabwn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iyibsshv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xrlbczbh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fsvptzmd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rtdgkdwd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ttwgnlfy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2cjccnhwc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iepsgyjf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vehwdfbi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mrkgzhec.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jghhkurm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ftljrfnd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2butibvcb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kbaitdvk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcozpkq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuburpxp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xqszlxzw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pqdguust.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikowwakm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qkyjdscu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2imdiduxk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zgtexoeh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hgisxpgl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gfkidmpg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gtkyifbk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rwtoaymv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wujijtid.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fiefbgpc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2trhvomwk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zrmwerjb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxbvznu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zclwhjdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zbqaqqyl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mookwyow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xfkuipxu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rfdaxiht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qwkldnfk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vxkfxdzh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2woiuudda.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vcgtnqjz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cauvemno.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2saoewdyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gbisknkc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2opjtqofi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wdzyomxs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2leethgwm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2awxphyir.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zmnaxhjg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mcfsvcgs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dzhlkyvi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ztststru.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xkyjlioi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kkusjyup.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sjekqlvl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uaxhrdit.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2izimpyyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wihjauih.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pzwnwttr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ygsxaenn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wdefelnh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qjjebsux.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2khqoukew.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fccaoiqr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2khdmhywe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fydpskqi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pvgegzcx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ursxzres.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2apgjaugv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2iuxutegy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kmjhreav.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2etcnxpgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djknkidp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hijprdvr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nisvocss.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uwksvxsh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sjekncsy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oakmermy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2oayubixg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2whxpxvih.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qoikyttc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nsquqqta.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2odebxrlo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bhiquikn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nkhftnir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fypblxjl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jmfedaxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dtepxkbs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zpwjtspz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqjudnnw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptacypvg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2egkrhnes.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oeeptfau.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bkldxwiz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ykeakwba.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bpbpvrga.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wiucnifg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nlfymqgl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rjjvgngz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2duusmbdc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whdixbwn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ozxcsugv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2haobbotc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2musscnpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihehnwdg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2otnblype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llbynbjn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qmhosogu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aggnmdot.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cuxmiszp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2igloeqnp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2awiqdzif.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bwrkhpvn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nneqoaeg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ickmcxqf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2japxzofy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ufosnrfv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rzsqbjge.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hzxizrak.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zbqtuesn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2igoxlmmw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjgdqzek.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jdujdvrf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfvrjdw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vuukgmlu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2algnzgta.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cflchpji.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2scrxpgwg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ynptzurx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kippboem.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysxdygzy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzsesyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2taggxcez.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zmjvdemn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bbqmbjax.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ouvlxikn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcyupfnu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pxgrlaqx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nlvnvjgb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ktvqocjq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tjzifaxs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2txdflszp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2htmravwa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbbcqnii.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jmljwjeq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lagmipos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lfggabmk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qoeempst.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jqbmcyxg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jvetfjqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ypgpdwcd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jtttccmo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dwkkanpz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kqqwjtkn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohybntxc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxfpauvb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iidoannf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nhzgspve.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idqdxtib.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lumxfydu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2koitpbcc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bzlwlonh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vctkbbke.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zpzvwdyf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nlrgfkns.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2syduvckw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eshcsbqy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hrzmtjoc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2byokxlkw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kynkvvpq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sktugpac.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrhlkdw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2heyouqcu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqnovu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mdukeluv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hfraquco.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xbpezmwx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2heldmkbh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2egsaybim.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2forpsxyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mneveisb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2klrbdmoh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tkwmpztd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ymadudzb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jamdzoog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvrxmpdg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2calfztqz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bvqoxytb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fkboycdw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rhozeecd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxkzcr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hbxqanea.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2minfkmxl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2reukvmpv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bulwsary.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2opqitvjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wqarnrdx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wfgdfykr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kvehuxkz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrrtcylh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2odidnuyk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zoaitqka.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqcopllo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfgmzppi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2klifuszk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vhlniorf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2azquipxk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iaihazem.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iwpamnkt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mpwcpbhq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xllkqixy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fhcsqbxk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vihhamjf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kkyaiomf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2czpbsmjk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pdhwbdoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ocnywmdt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sjcrzycv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzlexdqb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljnhbdrc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2txnemevm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hpjlgjyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2chrhrrhh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2heslxpgt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dyfnxkmx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qjdapwpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmcbuipc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ynhniixx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xumcpgxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yaldbwok.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fhcnuvcc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zaajjtee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjpyevai.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kxazdnvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rpfjpivp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2uhyoruur.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qeqvqvft.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zrofsxjh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fydajzpd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tjltuyqr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dmvmpysy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nljtviqn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mtbfrljm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txnhjopz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2noniomto.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fesaxtuk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2deobqkcu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bwlfbfqf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gymlabsm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ckxybgwu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vwyesaqy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eyrmksaw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdoceyp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxktygia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfdxpkd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2diapevnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rruiahtn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yerupchk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fwvamhsl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2izsdeyyz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2duyqdkck.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wexxvtws.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lquyjoal.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pfakactx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvhpwd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jaennjmz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ehnnmrwl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lqmvmdub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2preurtoj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxsetjtr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2crhowoaz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ihmezjnv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hpwsefeq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2krqdiokz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cjykgzrp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kxykgcoc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bmccifbq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vwiedynj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lzudsamy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtqehue.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2inoobojs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jovdtqml.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbqrah.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2emvpyreb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vfwyqclj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2otgeszqe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mjmusriu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2btuajwpb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2phoisnje.html


<!-- 参考信息 -->