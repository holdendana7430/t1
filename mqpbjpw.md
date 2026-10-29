代发 wailian999

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/giqwpueym.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gctbekdfu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gfjfmkwwp.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gvkzhctfn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/goffbcxcc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gqqcwlaou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/guktnewms.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/ggsjytruw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkjaouuaw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/govlfvymy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gllqkqvir.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gwfmsjija.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gtqzcfhvp.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/ghgobdfuw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmvwytpai.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gxougzsum.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/ggvkzktjq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/glsqexnmw.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gjibmzhvu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gfpfvysgz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gpcvellzi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnmnnqxug.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gggrhoxrd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/giggbtgxq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gcgtcdned.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gpwtdxomr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqzouewei.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gesueyccw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/glsaexrjq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gstvcdaqm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gjbctotci.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gdnmolles.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gmhbnbxac.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gudinywlv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gzxpqqvcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxrqfferc.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/glkuzmdpg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gkaoqitab.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/ghhmdeucc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gjhpdvftf.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gmxsvzaih.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gwbvetcpq.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gcbbfajpu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/geiicrpfb.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gsvyxsypf.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gjrabdcke.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/glfkzajig.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gjknxfxbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gpezujpkw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gvjjnkdcc.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gcfaivmel.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gurdndnju.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gewqvabst.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gpgvfnevb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gnxcsimtj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gfqqucmdt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gdnlismir.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gyhaseusp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gsggzslan.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gxnlcjrae.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gtlqlrwls.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/grnxexvpp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/ggvxsfhtu.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gbvaixmzf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gdkdwfwti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gsleejdkd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/goflinguv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gexwjzzju.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbitthnjj.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gutqrchel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/govscrwpd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gjlavjiyq.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gekvzibjg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gsoktoqjf.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gjolppcuu.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gtxdidscr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gnvhqgtpc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gamzmielk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gbtrmlouc.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbsmgzzga.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/ggtgzovrr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gxvhxoxrr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gbvwqhymh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/grbbvjoyf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gthhiqmok.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/glypbfcjg.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gtwqwdeyy.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gcyflsiwe.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gcrpuzgme.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gnbupccbh.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gvzuldmrt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gbqeabpzn.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gukzasslw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gftgngkhc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gwhwcbspe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gpfmuckou.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gpxgdnzpp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gbhripqwc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gakpiqvqr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzkxfyavq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gzagprnrd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfspqqajv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gmvfeuwvk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gjgqyrdcd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/geuwaasdn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/grbcxbamm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/ghzdzdcjy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gbytpbrqh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gbwtinqeh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gsmbefmwr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/ggrziqjaq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gndnyibyk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gahsoibwr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnsnrxhkq.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gtoorvolz.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtrflqhsp.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gxfdsotwt.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gjqfspuje.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gcttmxaba.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gefdqbioi.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/ggeckbjba.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gbvbyuckx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gnvjsnjxd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gwyndqngq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwvytntwp.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gokfuqbbj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gjqinqxyq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gkluyznni.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcfveatgh.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gsyljxvnk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gbnpvdvsy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gjkzcplgi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gyfghgmbh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/ggdcrudpt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gsqzqzbar.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/grxqgbmvr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/grwafvhro.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gfpcgtnfq.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gerbreqom.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/geodxoysi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzoeexzww.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ghmnvnglh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gdkyyuyem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gofaqpwpj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gybyniaba.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbnaujpzo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grtkhcvxh.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpxwiovas.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gndzusqgn.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gcjomdsrz.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gnmixookj.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/getqhjmlj.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gcvhkmpls.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdtddhneg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gyahgpvcu.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gmvxzndky.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/goxagmzhs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/goadpmiij.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gcayqburq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gcgpnvdjh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gsinnrlrr.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwcndyjtp.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gqcgvaizn.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gltwqwkob.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gspfhpmnh.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gsulinxkg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gnhwwiyvr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gbpcqgnqy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/grmxhldrz.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/guvtykvyl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfloznsvm.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gxyqnqnvr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gxnbzvpxa.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnxtxsugc.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gsctifmwm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxbtyju.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/ghtvtfirr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gwecmyueu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gpxodildl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gvllzegld.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdfaclaof.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvyqepwis.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gklqexujt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/glvvpzyol.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gzyfxdgkn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gipklqoyd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gnmenjkak.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gugijpuvv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gbsgsfueu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gurgrmrhq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gacdxtdwg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gnsabwmdf.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/grecxzgss.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gdbwojxeh.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gwbayhgqm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gcynrkoao.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gsntqzshc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gqwnycpnv.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gcnbzwvrt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggktavaol.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/goqweqvft.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gdcgdtmim.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/ggymvuzdk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvyaoiohw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gtqqigblp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/giqajrnnr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gcaidlcvu.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbmhidews.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gnmykilhr.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gljpcgfnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/girknpdwk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gmgfuuagi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gdkzpyuoi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gqwezqdkr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmpvoutjm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guekueplb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gfbdvfhey.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gamxsdwbo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcyygyulu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gzpuuckho.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gopfixvmx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gglpoyxku.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/giudunqso.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnumgsbqs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzkjrbiyu.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjibvaoua.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxiwxeinh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gptmjjwvi.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gshrwdvql.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gozyhcafm.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gcseqcdno.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzsgbxhqw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gyrqmbjet.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/guiukrykt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gcbveosve.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gkjvommrv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcklsjmra.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gwekcfzty.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gioxowwpq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gasspztlm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbkgywqtu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggjlnezlx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gsiaifgjo.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gditgehji.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/godbrqdza.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gwchxiyal.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gaumzxdea.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/guxvczgbh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvznfzafu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gdklshwdp.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gacvyrymq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gbpoeagkd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gfcckfztn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gaecbmpwj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gwhbjhesz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gohrozwzg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxfiluw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gqtzdtyvp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gisgjsmfh.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gfeqffubk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gogznhssc.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gktaxggyi.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gqmsxjqtf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkoonifov.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gjwsmftbr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gxjpwcpmk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gyirxpcfh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gwrltuvex.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gciymgqqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gvgxogsvt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gsjdfxdsa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/ghjjhxtkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhemefg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gsqrcaggs.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/goimyuzvu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxobbxhyk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gmqcsxaaq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/getbcvzpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gtkmsynqo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/grdsldlck.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gjyhycdmc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gmymtjozl.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gheamhnos.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/ghvibeiqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gkxzekhfy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gaiokntok.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqzvgfmch.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gpysyjsar.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbgupyozx.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gbykcbgkq.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggijwdgoe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/glkywszxm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gxvzdqodv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gigghpwty.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gglzjggmw.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxnhcnm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/glazmwpmj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/ghcgazdve.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gxirvccoy.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gsbscilvr.sHtML


<!-- 参考信息 -->