代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gykkdnwwa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gxzrztggb.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/ghspbjwsp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ggoujnook.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gquwqphwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gzjsehafq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbkfynw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gdeiafcxj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gotglujmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gxwlcmvig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gkpskrneh.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gauglprqw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gzmiznhoe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gplvyrhge.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gbxmfzbrf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/glulxdxny.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwcxwue.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gifxkwotz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gchkgciwh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gjgrifidx.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gahgvdmng.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gskrnfrxr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gletbmasp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gcvylclhc.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gmimmonpb.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gohtjpmhl.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsdeoblse.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gyibuzwex.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gsciwdikt.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gmxdtvckl.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gawotsjoy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gqnimphph.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/guqcpvuva.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/glpstyvec.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/girxvbtyr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gdoryhhgp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/ghwqjbbeg.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gsaohdcef.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gipnzrxhl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gilhkligb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gbowfoqka.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gttqqnirp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gsinatflt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gzqtyekte.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gkwerwkha.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/grfbozckz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gnbyakxln.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gotekbpla.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gowarfsib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmqwvhgha.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gtgrqobev.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmtyfujsj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbmqcrbbl.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gxbuvrvsz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gknntavff.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gncoqakpt.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gqrguxasm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/glovofosx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gcitawdlx.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gkmoqkonr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gmnvwdewd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gmufqfngx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gvnjmghri.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gavgdsplt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gowrgvfwn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gopqumnaf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gtwafbtkh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/guxyboilb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/geyayacje.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/ghqoafgzl.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gfvlcorrw.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gciohqdaq.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/grczobzuz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gvgresglj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gzbtubqqp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gexfwdqyl.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gzesnqyky.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/guemgflie.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gsmnmiara.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gkngluudr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gvehqkiel.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gmkvbjceu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gaxmzywhg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/golaqkcda.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gpqjylmtw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gecdfntsm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gabkakgbm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gllfhswsb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gmsbowsxa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gfwhoeggv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gybrrgujx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/ggsqanxsy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gnubvqpap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gfabhspzt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/glnlvtaau.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gbojvahmp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gtchgghkn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gjinjphxc.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gusvkkkax.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gbgyeksai.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/glhcyxeev.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfmshmqlx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/grsbfsptf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gxqcgozfp.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gqqiocqaf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gluahuqwy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gvyuiexks.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/ghfrtbgzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gpmintdlq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvxxmihlk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gcsttgmxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gwkwhrtew.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmgafumoi.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gtshjxcoa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gppnkaymj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gsdgqoyhb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gnjghrree.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gfgtdjkjh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gxejnspva.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gliulbhql.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gsyhnrucj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gqjkueics.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gajnazexg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gkzqltmav.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnzxbtzcz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gcsmtffof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/ggaqpboac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gscwsjbbo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/golanecfa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvsrvvjnq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gkvfsfjdq.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gcvwypcwc.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjymhznyu.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/ggdueeelx.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gqiiyfhro.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gpnelypjp.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gnxszirbu.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/grwyipper.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gnhshmakk.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gvdtuwnma.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gvpfsoolk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gelmvyjyz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gdmrjfeox.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gtecdznfc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gwofpjuii.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/giyegamfz.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gykdcuhch.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gqicprlan.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gharjaulv.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gnhhegvpj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbqxcpreo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gdbfywojh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gdrsggtht.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gsjrmbmbz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gyqpwocko.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gvcjbasta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gohfzdyyu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gmmqyvtvw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gfiznqeof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gnkzfgdxx.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gtuqyqyms.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/ghpedxsyb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gwhgirpas.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gpkaxpwtv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gjlwlypic.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gkfrescfy.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gqguydnzv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gmegftvfs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gisjqidyg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gidovoujh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzcvtmoys.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpaqduypk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/giogynkkw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ggdjkyceo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gdpjlsppg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gohvtjngs.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gztweobci.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gthbszidd.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gopnchxdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gchdvgxzf.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/guusgaqrs.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gizqwjhov.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gszwoqudo.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gqwivvnqg.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gzrqsreel.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ghfzulbcw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gfvrgbdmo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gnlpcvsbt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gikkqvbeq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gerfuutlh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gpefxrlky.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gockkwwju.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxdepstci.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gtrhuqsxv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gqhlvrlcr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gggbbvohg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gmlejhjum.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbkzddmnm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/glmgvxydi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/giwmuvnnv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gyykclzoc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gtknotylr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzjreauvj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gtlaahfdm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gthgdohpz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/givnzmfae.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gbmruzhtv.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gkvdisrdm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gapxuonml.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gkqibzguk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gesnkzufp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gsbyftiuz.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gxmtnlkle.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/groeeeues.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/grumcheky.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gjgqqamfj.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gtgjouxjy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gyirhahyc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gflxwbrsr.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gxbdxnxty.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/ghopxvdcg.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ggpzapaxu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmaeqybam.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gadhojxkf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/goejufnhp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvstkucub.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gfzmzylbg.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gchrtgruc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gbnyvxjhx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gjwixebnu.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gsfcywwap.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gmpaernzq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gmcpfhlru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/ghybysjya.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnijuhp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdfvflkzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gaulevsoo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gcbdiemgh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gutrqomnn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gwuosufcn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gnteluobb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gfyozrhpb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/ganrxvfwl.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ggsqhfheq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gksmaxaxk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gmzmjpbxj.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/ghivfecus.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gmtsxzpel.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gaoezpuac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gfslqywfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gaapzvabo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/genaiifja.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gqtdzjdty.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gzwxlxwgs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/glzdxkztg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gqogcttge.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gyaaottsz.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggjnfjlxx.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gjlbgccym.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gpzmnzobx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gyprsjbcc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghnskskfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gbatrjleq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gwchayuzb.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gbfciaszm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gwzqmvlqy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gmltytamo.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gqohodrkd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/grhnlbfdv.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gzpegztre.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gekpzdmto.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnobxhnqq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gifpsudil.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpegxiuqo.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfngszprb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/goansmibb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gaxtkfalo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/grwsjvkvv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gqhpwwjle.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gbydpvtdu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gjlikrvcc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gjjgagjcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gcldqcelm.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gbafvfpgk.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gtooifklt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/geisiosoq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gupzyulka.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtejezmgq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjvldmkwx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gzdvnhsuh.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gwbjmwyuh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/ghbnpmolk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/ggbezlveg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqyifcudj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/grvehexwg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gwftovjnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gvhcprckt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtwlmcldf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gntmnwism.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gcvwbwujr.sHtML


<!-- 参考信息 -->