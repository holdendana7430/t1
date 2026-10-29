代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/guhjvhszk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/grydjfdat.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gfbjbhlru.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gszyjfyyz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/glzawohif.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gtpgcchhw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gfgjjkbpo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gjpanuqup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gusayidvy.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gglkjufqw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gelkdfbvs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gpxlyingo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gkvskxaic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gjzwgkxbh.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/ggfjhbyud.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/grjtupbjt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gifaweyyj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfrnnhbce.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gufvrlpwd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gygjdxsfy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gzuwafheh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gaagfpcbk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/grmzdyaau.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gwtmqutov.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gmxhfeybe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gxknqrlig.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gryqdugma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/grflofbjx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gdhweobys.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/ggiqtfhwl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gxycretal.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gvuayixmf.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ggvzfssze.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gtgnsswja.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/goilubsua.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/glrsebuil.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/goyratamt.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtzhnchcd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ghjxuldzr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gcjclppss.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gihuitodq.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gjfrfvahn.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gtdyvpkyz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/guyjdcuoo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gfcavkirp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gfqmgexxj.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/glmnhlwly.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gmtbnvuux.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gchjuqafi.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/giqteajqi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gcspjmxze.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gexvnzsxy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gjjrumnhu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gfvbtdtkc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkzigihow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gagoeeoka.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gqufqmxcb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gsghphskd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gojxikdcn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gxhdbcrzm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gysizfzay.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gyyzenwlk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gdyqeuoej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqchqczep.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjjelbtwq.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gmtebdbdd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrcyyigo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gvvxernfj.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/glcyhyzre.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gixwdyetj.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gkyzwnqkx.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/goqtprxrd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/grhhyqhrw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gkdlyrnjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gitdpenaz.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/ghmxtfojf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gbycoftrh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gxkjlolyk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gdztaehdr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxsujovh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gbxlchfyg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/grevmjxuz.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gqzloujbv.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfstnsvoc.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gwddqwpjh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gzdjopwon.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gdrkujgcx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ggsyynesg.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/giiechwcp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gkdmjdpnx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gqtdledmq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gjhimurmv.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gppxwqdyj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gfesdbhdh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gjwdgctht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gywsvfaxg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gtavmgkjj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtgpkmcxn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gbdcnxfpg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/glxkvbvjz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gqjtrvhqd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gvdubdqyu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/ghclrkvop.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ggeekhdco.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/getnkihky.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gbwvzssny.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gwgdhufyn.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gesprzkdu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gxvtpgppd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/giuunbdjy.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gdyolmjsg.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gtbyqmjot.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/grmqztfxr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/guumsfmer.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gwkvhhkpf.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/ghvvzgjvf.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gmbhovwwf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/ghdbyomln.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gfbfalnhq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gynzlneps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gonhyxnnt.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gukesunyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gvswiolvg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gptczqhwp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gaihtaryt.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gfbqlvstu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/ghchpzjho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmwhwfkki.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gydtggpib.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gcphmupuk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gwabqueke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/guwxzvqzk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gigtfscec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/garknoxrv.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gvxdhawwd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmegggqai.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbfguwmuq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdtqcgzbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gfkbcgeee.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gmltpbryt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gxaykphzx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxlxlwmnp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gpgnnuokh.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gsyuuozic.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwposemqf.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcbfmfdgr.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gbovmqiqi.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/guxonpdst.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gbjayhwdk.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gjmqyeqvh.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gdmfyhwyr.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gelopzgqr.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gohmzgqat.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gjmxrxtpk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/ghiqowcce.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gofiyycen.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjbpbycpp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsdqqpppk.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gvdzotjwl.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/ggzlecimk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gpadnrkmx.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gybwibxeg.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gxhxgdbqh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/golxttxxc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gykkesvqt.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gayvwelqd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpohwwmwl.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/glwtnmjyh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gvatkcqjp.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gawujdkmk.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/glubcyqdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gfsykdtuu.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gcidhrwwx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gwfdcjwxd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gvyqvivro.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gdqqjffok.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwazjqknz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/glidqpegc.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gellljbbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gpylhotho.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ggfhbvdoc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gnqeyxucn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/giiuxmiag.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/ghcdmxrxj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gvyxdxxlt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gprgufzhy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gvsvuodur.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/giyquuihy.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gadrbkheq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gzjvwtyao.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gdlwxpwhl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gvnjwghla.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gtiryagqc.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gbgttcoue.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gewveaoeb.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gyfvrjwfk.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gfnummxep.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwrtruuuf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gtfwepzkt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtdtcvgvj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxazgpfvo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gzhiihkul.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gcnsghdgv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gikpdiozl.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gxmgiioex.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkwmbiosd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gwueccmoz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/grvrntais.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gueqbaqde.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gxnptxjfk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gjbbfhatp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjfkflmh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gvlvheeah.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/grtdqantp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvqlarmku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gcttnotvl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/glmdxqtmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbeyvkmrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gocsvuucr.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ginmyabcf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gfhmishlk.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gyemtocmb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gtbcsgguf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gafvhapgr.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gfdrnjejs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggfngkzwg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gajhywxcp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gldecfaeo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/geoyktsxg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gtfmpqcok.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gdaalzebz.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gehqksoak.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gahxuxupj.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gbiiezqcu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcbbvwjfz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grxzlihdf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gtmdgmqqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gggtjrcnd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gpjkkebid.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gdnfaerua.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gqckpthkn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gtfzpotux.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gtemgawjv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gphfoepgk.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gznjpmckj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/geqlzsdxs.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gznqqyugd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gdkvqsskp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ganfdofaa.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gwmbwzbgp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gbresekll.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gatalfowx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gapzunpge.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gzegxkukb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gfoythhcz.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/glxomvipw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/ggomjpchq.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gkruyfcir.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gfkkbwsmw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzayhvcyk.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gifrtdynt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gaztipmxg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ghraplvdd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gqaxzfyfb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gppgnjpam.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gymvjoovj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gzfvcymki.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gsthbckth.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gqapefamg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gaxujxrbz.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gyufulaog.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gnugpexup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gcpiosbgb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gabopytca.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gagabbkwv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gtkyytucs.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/grjoccphm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gqtyravfa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gdttvrcqd.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gxaglrzmk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gboayqrya.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gdhhgqbrq.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gchttsash.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcqqhnt.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gljmszzgd.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gaynueuhb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gphgaeaio.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gzjokcjce.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gxhlqlams.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/ghqlqeazq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjcsmjtri.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ghanpmnli.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gwufarkco.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gogwjtyvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gwyncjlud.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gjtsraivp.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gyforelhc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfljrpcox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gcsifkvip.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gijpidyau.sHtML


<!-- 参考信息 -->