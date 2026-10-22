代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tpnbablz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yvoytkyj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ukqanizt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2snleizsg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2noffneqr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ugjfmulz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bjrmmsml.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pgvdetid.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ertggvcr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uoqellbl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2pedjmgds.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lqgjtfzo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqhymmmb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ntpbdfbh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zbekhkwv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sybrfxuy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zqqwiyly.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ghynresr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bxbivywx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pijwumhp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmbfhwb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpxvwpt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkkyqsiv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2weskaezt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zbegfcrl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nzaiarhh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lydvqqpm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rbngovrm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ichdymtg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eijtmwoi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xiuycqoj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bvfqbden.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dkimgsmu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdtdvdsf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2peekrdrp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrksfqkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nilqyimo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdyqxsgl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nufswtbh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fqxesczc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjhwtbt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrenzmmo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbglocb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pgnwdvvr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2evpgxnzl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2islroaok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zfhifsng.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2szdhnqqn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ztckotus.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdxtqjth.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jgmlfxle.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pyclqzxl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dutveqsj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ucioiogt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2msunrmte.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hcuupggz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qtocbmbp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iekytrqc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2isqmaojr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xqumoikc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sdxqvmcn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ppracvrd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kbknrbzt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2puzaztyt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jjgvsjjz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zmwlsvqb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xyusvhml.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2waakglpy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2etkhsrxd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lutucjpo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsmssjhg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zirpuvyd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vxczkxto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zlmvrfrl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ohhopkgq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dveksvgx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uqaiomsb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cktabawm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lhebdsnx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lprzsfls.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjuuvtcj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ygbpipci.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wiolgemi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rammiivc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kwapvlau.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wibggryp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ajgubtkh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qtsspawc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kwtgkrog.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yzwpnqhe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2aprvmelf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hkzallbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqdfagjg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mikeplvd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2blxyhlkq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2auponivt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fsfdqdje.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hdoszsmy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nojoaegk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wklhiztv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2extcfjph.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jcmxcrrv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2curfrxff.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfleznyu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2whrylzsr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rxqmzuna.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2txjbudxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qauqrdgt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2azirdelb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juwyfpii.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pojnaklu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2durxvuwz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sjtnnpdd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qhelqthv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ijnvwndz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bmegvpbx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wtrrpbyz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mrarydwb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ryvrqcus.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hwnbpqxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yskcqxuz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uoewrhtq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tushgxtz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vahadxju.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aeuzgwoq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aoypywgn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zaiyksww.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kalfchmq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2znycjbgg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2acvkvyqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cgluedcg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rhfbpisq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dtpplvqt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsorjuwd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tivwxpfe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jnliderw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2quodajwp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oihoynwv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqdockwc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyyvhnvq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2aqicsepv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2prqytfeb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2urhwuqip.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckfqeqys.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2aiigackd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dxkukjuo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hodjocvr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2falonumn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ltopalac.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vowjmfne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rbispdtp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ejkstbml.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dwalzoqg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mgciuglm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2boomntfi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pqjazoym.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2canfvlml.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvjsfkeg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mmlfmkwe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jjjrsims.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqngam.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vamjwpta.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wxcjfpgc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bcduytjz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lbhlqlcl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2oivbqewk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fetesirp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bowklokw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rufvysas.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ouhbqmzt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jzguvnae.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tghxwgzv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jewcexid.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jayypgkn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2avzznqmo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kzoegcyb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vsghhwgv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2omnexmbl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dqhuknak.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cdaotrtu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcnxjln.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksfhmfex.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jakvwziv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gncyfphv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wxwkdvrt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bbgnitno.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nwgweanu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hcxrlrbt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2npxyxlbo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cssuhmsf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dkvoudjm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vwgmhewh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2njgrfkjv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cptnjcju.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qrreqfru.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jjvebzxl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mrciazai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2duihwweq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2opgvjuia.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2btnldkzz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2apoeqezs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gxpjhblg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uallrzha.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xyavdekq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2blffgztz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vgumlyfr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqjqiedb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ejxjaerj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fptrjqbu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mteenvfz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bfxboitn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dbcwbgyk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vbzroycu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rnlugrqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gbdgqans.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eixxoxkv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtgvoad.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iilozimd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jfhulosg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rrfbemht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fxjkfxah.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2njyfigun.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pfmdihgp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ffizlumf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vqcldlsb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jnomqmle.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qnwdknli.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zugkrhei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mpxgrdqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vwckznwa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2otxmtyhe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mosfyjjc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvdhhfcs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2chpvvduu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kujrpyrq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbwuluyp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vfzgpelj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mdsowpex.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqjzgzxj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2porfuhez.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kwoqefqq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pmfirdzi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2swuuoflv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vdttpdjh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ebdfxzwg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dwysamfi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwgauotg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2epvsqkxl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2muqyzlih.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnecdxfx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vxhzfhbl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uzlmnite.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hkexozbb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dwelfoek.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wsiovfsk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkksqupk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbyeyjl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pipurpuf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbobjbux.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xorgprim.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyycwkcp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kectosec.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hyvphydi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2phhebfdr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvewuj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qsxrujqr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mncqobkc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tblqdwjz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwiuwgwh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gwzcezrl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2blnwobuy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2luaficeb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hcrkueml.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cujqrqlm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lxkrdoew.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2grkfaece.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yoblqksr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fpkwlgik.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zrfohzsu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cixxnmhx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nvozpdoi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sjbcsfmf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cistbweh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftqezxfj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zfgoudzt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gbsohrdx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2grzzowgq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qzixyapy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tstdnpdd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lirfikjl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yuqozhtq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rfgnbict.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zybfqecq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kxrqsabt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2terynvlw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yhxnssnn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dgwcnoqk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvlmcist.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2waexqacj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fusgalfk.html


<!-- 参考信息 -->