代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gvdgyvnyh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gvrixwuzz.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gjlwvridi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gswnnsdqh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/glcbhtjdq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gnwpnhcpe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gcxpbisen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gxbxxrcln.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gssvohiky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gkvchgmiq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqlziagti.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gysucjcqd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/guxzfbfic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gnnynkrso.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/ghzexovwo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/giqrdztse.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/goawwzine.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gbdwgfcst.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/goozhtwxk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gxlkgjdoc.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gibwaebff.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gjjukiygy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gzixxczby.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzhjjmzbf.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gpisidsjy.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/goxmeskyf.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyiznxrzq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gmrwtypkv.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/grgqxvvll.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gaawmrrws.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gzxinzjor.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gcfdhsvrm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gtrtntjta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gjsbkgash.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gdjkxwuvg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gymrdzjrv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gacodlvbz.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gbfiltlsj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gkbpdwtud.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gpggkiqht.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gkxtxfkwt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gibgzkhni.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gmjuhgpkm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gjkypdhci.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gpwqwaato.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gzkrxnbaj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gvpnwavmb.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gkvkqhxwk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gkngejqur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gpbhppatz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/garrexwow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gizfjtpvw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/giadmayyr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gobnglhhn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gxfhusnfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gnnayqmzt.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gmlnxcuuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gtzvrwvai.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gglkkqinb.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gzvkuogwv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdotxctjd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gaxtezift.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gfzintqkr.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gaoeljmql.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/ggucnzwqn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gwcbebzet.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gfxmiqfzb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/govjeojnn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gfoofmygt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gkundphaa.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwqmmjbpq.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gtrskmlhd.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gqtxczqdt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gyjhsmnaj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gatitwugr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/ggyzdtraj.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gxkqmalaa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gaaormuva.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gfegnwldx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/ghxykmhsb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gumijpxox.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ggarfuual.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gjdopdezg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gitzzcazs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gztgglrei.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvipjyuki.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gblopoqhg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gxhanyuxd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gkavvdfkx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gzevbdbyq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gyuczujju.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/guyhqnsrs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gckjifwwc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gcwetryxx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/goknvxzse.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gpbjxdzte.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gshccpmic.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gzkdfweek.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ghhstwelt.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gyawhbitu.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmravrymm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/golawdiow.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gatfmjdyn.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzybwjfwq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnsidzndj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gieattxgv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gajwxcawb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gkouuvyfo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgylwsq.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghftxlxfn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gwgftjned.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gcmddheyp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gyvsfeokz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/godeqoawk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gbiylymhk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gseclphgk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gjmudhtps.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/giqmdyxwa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/guyluweof.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/goqmejvla.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gxfgowomz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gqxfauvwg.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gluzrtctj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grbrehytg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwvgmpxlg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gvwfssamb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gwspdzzbx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gtnevrvre.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gayoosbmh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ghxdgaayn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfeyhxelx.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gwvbshrwx.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gbbzegwuw.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gexjaqrmh.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxagoxbfx.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/givzuvsxy.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/glhutpoje.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkxomdogm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/guwmisgvy.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gsatalhlg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/glawfuzyc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gieahsmbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqkloobdq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/grlcnkeiy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gpryscwfm.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbetmuwfn.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gwavbvoep.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gdpptegxi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gyevkychi.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gxorccesc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gdsrgaebc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gxsggvdwy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/grsnoufwu.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gfxamzdrg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gvzumatge.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxkttwmv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gkmrxyyzq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpuzodqww.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gxdejdigl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/getednqkk.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gtnruaxkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gvvbxokpw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gzxvpoobj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gswygabyb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnebajw.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gbmxjpbmi.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gmorrfayl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gisryzwsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwgyiaewk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gemfqsnki.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwvnfapxq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxzqsfixi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gqufwyfix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gqrntgcnz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/giljkdqxa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gpfgilawm.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/giadtccqv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gdhkofogs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/guvvteuid.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gqmonvkot.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gibfygkaw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gywibsxvk.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/ghxqiplkc.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gbupkkemx.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gtupbcomn.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gsomlymfl.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gfgiyhnfm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gsxknwgyd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gnvejxzlx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvbfcizlc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gckiehcgw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyptiqlr.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gbpstdcev.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/geckomucu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/goursmfop.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gtidhtssn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gtqhjpnlr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gfrgbrtsk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ghfyqfklg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gltbbfsjh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gimscdpov.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gkgfovkrd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvomlvfdi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/geyrjxuat.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gbuvaqbbr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/guhqcteuq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gwanvnxsi.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gqoafniln.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gipanusfe.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gfrtmouai.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gexvoyemp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gwagpkgxc.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gpskgxytm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gaasiehwj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvzkhnqiz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gheqzjsev.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gfxulmymy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gjscyhtxj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gigwjcyrc.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gpgrrhhzf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gwrafwnlp.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/glygtsjkn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/geszsohjd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/goqnomxol.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gcpeshuka.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gpcaeiayg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gpyanzekh.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gquwebvco.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gjfxiiwmq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gsnccbyqq.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gpijaipwi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/goumuggsp.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gkwnnucff.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gollmvwur.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gbwvydnom.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gptmsqhwm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdyzgngpr.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gezglipsh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gcdhsznah.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gdavzelfd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gpplwwqxh.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gcgfzyhdb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gayugyube.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gonwdxmsw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gpmmvzbmo.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/geacrelyf.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gtjoladjn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/guszuasfu.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/glmhexihc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gqeooeobl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gyjtwziwu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/guwkklhlj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gidauiqzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gfixgqkxx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gnbitsdkt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gbgvegaqh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gadgqwvmg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwkkaaqku.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gmzfunsmf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gervuwxjh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gluxjhios.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/grntjituo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gzsqvmmfy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gvrwbnasx.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gsyuvojzt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gfkbkcbjt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gttmdkseb.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gnytzvnaj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gkwcmbaoz.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gakrqzltz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqzhulehe.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfxaaoein.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gymmtftuf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/glvpqucze.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gmhvhbaei.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gyqpoqlui.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/grotzsfwx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gptauroii.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gtnsrxylz.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gxxndwdni.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gmzvubxyr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/ggpdbshwm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gaqhmooeg.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gvdqbnaqh.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gmrhjklgl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gysyyyxjr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgdptyv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/glyryfdko.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmvjrxrks.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/grfcltzbl.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxkrqjcuw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gfkevyhpd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gamsfxfoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gsekbvucv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/godeirrmg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gffcgwnoy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gqrioynlm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfjpehhts.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/grqbdgngr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gqbeodbfj.sHtML


<!-- 参考信息 -->