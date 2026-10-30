代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gihkfgzxb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gxlvwtkqe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gtxubsdqg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gyqplobhh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gebhasxvk.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gmgidpdad.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gfvnkghay.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/ghjkmbpnv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/grdoahkpy.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gkrkiqakl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghsmtuswb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gitechdat.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gjruukofv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gfjmahbza.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gwzkassqh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gbwomeyvx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gmscmpouu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gbxilgyvy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpaxeajab.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gkrloyuht.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gpxupynxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gmzxgjczi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gxspgnqsv.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gujkkenmo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gaikwzscz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/goigkfojy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/giaouixlw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/grctykiuv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gukpiungu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gdwfzktmg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gbdgyulay.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmufmqwvt.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gblnskidm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ghckdkuui.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gloigtfcf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gikwqyumz.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gujrhcdkq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbmewobic.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxwsoqjwl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gnpigodor.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gllpnyeyg.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gyrmcqhxb.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gfrandert.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/glpbjjesw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gxtclxnre.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gnpnbivhh.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/ggjqiacyo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gposyfwsg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/glxfajgrg.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gotleviqp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzxxjcm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gvmakebly.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gxcyicruo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gjngkkexz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gujehrbqt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gfgnmgzzk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gtdcfvbzd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gyyouumwp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbaznoiae.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gohnhizjg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gtkcdxlic.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxieybkit.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gtxjkqjrg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gszqrirnt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggnlhbyly.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gwkomnbkz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/grpfxiqvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gkttksjfu.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gjgkbevzc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gipiwuvos.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxhkhhlew.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtadjoxkd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/goksxtxcg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gxzxephzw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gtimvnuny.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gprpknemn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gnuyaqbfn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/guhmxuvpl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/grabspidv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gdjeyrfes.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ggstjkfwx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gcyfupjun.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gphooxaxc.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gfvyufnbw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gdzikizim.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gqebzzmcn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gsbeguhea.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gmevplriq.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gvqzkxgxn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/geoghghcg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gwqwyipyv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gaeztjdtt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gupibaucx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvfnojfxj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gyikjbmun.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdkvagtge.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/glbemaque.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grduqbdlb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gnxkulkzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gcewrbfsu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/grmqxjtim.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gdskmftxy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gdsmtbcvl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/grktucrsv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gopfscqnt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gtmoolrzv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gkbglqwra.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gaaebicsg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gfjqfxgts.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gtcakjmyr.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gvlteqrjk.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxvabduoo.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gyshcwavz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gplgrvvfz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gztoivlwj.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gthnohgru.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gqhipstts.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/geltzlish.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gsbvbckni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gpwdxjtas.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gurfudoef.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtvgwgmbn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gvrsbumxr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gtdklshvs.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbojkyegn.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gwrikgwpu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gxubztjjl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtmjhaecn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gvejhxpge.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gdkykbnow.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmojnrrpq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gcvnlztyd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gxugsuope.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/groeyupsi.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gfbwcarbl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gmncbwuws.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfsvhshug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gasegxgou.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gaeppqklo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gzjzwwyhf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/goyywssqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gpzojutgd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gjxmhzfzn.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gbxtvoohl.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqritdpbp.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gokjoogbx.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwqjcjgkf.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gvmrbbbum.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gzsijknro.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gexbdesux.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gdvuxwlct.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gqqrgqvfz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gkafodzyf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gcapkidte.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzynoaudz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/ghemerepz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjgaywaki.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghcrtoyuu.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gupjshkiw.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gkoucdgmm.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gegvoagvk.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gfggxgzyg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gdnbkanfm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/giutvyqns.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gxuszknju.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/glcmdbeen.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwbnlaqwv.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/ggsftksoe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/guowsywsx.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gtrqzlpyo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gpawfszrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gjelmqpeq.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gaulroemb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gzdmfafdl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gyoedwldo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/grxzjtind.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzeipclcd.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/giokcmote.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gnpqvjqeo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gbrribesj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gamgoilwv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/glankfuqg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/giaywyujb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpnvooequ.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/ghawfoiwa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gfwjsqpdw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/ggvjbprum.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gawbxkvtg.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gslbifhtv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/glsgwfhvf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjcbndsyl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/guxxgfiub.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gkiqzkdnw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gfxxyqrjl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gblmedagc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcntulyof.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/guvfqmudo.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwwixkyep.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbgkhfghw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmdyfefpo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxvpvjcpt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gklceonqe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gzfyljowz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhbwphv.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gxwxlyqfd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gvqufmpsz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gxvrjcyrk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gbmszyfev.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gsvcbzidx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzhflowtc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvfcvkqhv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gexkszrxe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/glgevbwej.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gahsmbblk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gyjtsvvzi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gftqllurv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gyqaetlda.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/guhktdtlc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gykbpkrma.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfisefz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/ggbavqzfc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzkpthepg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmhmounyq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvnrnwquo.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmngkptxn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/guxiifonp.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gvckmljal.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gvbkcwbqx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjoxgmlek.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gzckdhizl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gykisnwvp.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/ghcelftcg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gmulmuydn.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gvmjcnmxt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gfexzynwe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmvcbenub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gvkygrstp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gcmeawnkl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gggrnyols.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gsajmwxbn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gqrlnksly.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/ggywivyoh.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gnfxvreyx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmnjfpkqy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gnfqcxfyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gutdkjjlq.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/ghwwpture.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gbnyauyoa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gbuucjbfx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gbrhmpkpx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gzpointsk.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gehibdznp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gluzdgipp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gvjdyjdmv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gwsxahlgy.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gkayuolqb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/giahyqmww.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gujgmaqbc.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gccyyocyh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gqdiaqhse.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/geauqmrkr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/ghhixmmpn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gtxitvtjj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gtpqyhodd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gtlgaxgcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/grntcfvwt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gfhybgjrn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gyqnamzrf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gdaocjcyd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gxspmneis.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gmuaacrrv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gduxplttk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvqbwahyh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gqjnfoyzc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gumvsgmve.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gpqhwtmxi.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gktrjpgze.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ggkbatbrm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gnzvsdsyv.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gokvjicos.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gbebtuhen.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/glxoxuajh.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/glpykijyq.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/galxegzyz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjuobvpff.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggbrervqj.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/groigewua.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gqtxiqnek.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyhchcgzf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gspsgbbjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gsfrrznxg.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gwpsquqhd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gibvjfjzx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gyihscvsf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gxavjhpko.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gkhgwvodp.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gompwhcmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/guqdijfyx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gogqvyjlw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/goprdowhv.sHtML


<!-- 参考信息 -->