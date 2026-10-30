代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ghtwjleoa.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gnhccbtrp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gijhtcinn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gxrhsfuuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gpywhjowo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gatijcvar.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gadswwjxo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/grydnqxli.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gahvyhcjo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gwkvaxgqs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfqmvttek.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gaxkpyejo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/glmvtsjpr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gshqmelda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/grkmxpgdx.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gkolnjpcl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gcvxfqzqi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gakfgxmyh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/grjpcqjbw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gluhwkkjd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gwwlocsdr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gsqzufmzy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gpzodstjo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gnfofugmc.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gegvypton.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gliodvrgn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gfxsimbaz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxzoanghw.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gyvwcedsn.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gaaylavik.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwzbytktf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gwejnwgat.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gewvaogjm.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gqgmhcdds.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gmliediwg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gakbwzolf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ganujfoct.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gvzdyrhww.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gsnoinotm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gofjsomjr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gplytappz.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gdgawbcmb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gxdbjtsuf.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/ghhfbnska.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gwnkbyyzs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/geooxluyb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/giufzxcuy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gfelwgchq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gpupplakm.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/guyamdbqn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gnalriqnl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/ggfruzifp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/ghtiujkor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/grczuyjub.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gvqjprxlq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/geckbqyzj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geqkgoxas.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gzbyeyvgl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gkponkjqc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gfnfevhrd.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gomezbgid.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gcbashvqc.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjkocdpkp.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/glhefzgjc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gaaxuwzll.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gmjswbtdd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gmcleumrm.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggkwcnjsr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gydzsyzro.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/geptqeclu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gcsjwtbcr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gwraapoyq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/guutlpxbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gpenxpcbo.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gyxczrpnp.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gxnsbgtdj.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gzdjlnyng.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gygvkivom.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwyooskel.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gxjsmvxgq.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/ggtpzshvv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gymiffyid.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/guyxxyaiu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkdvoohka.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/guzyftgkq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/groquksri.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/ggxofrfve.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkzszgpze.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gcihdfrhf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtmbypncq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gsliauwcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gajptncrt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gflxfrukc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/glckopcwm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gdcdiobak.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gariosiwt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gmaaihcid.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gpxmdgzwc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/grojtjlpx.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gslitwqwq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gxwwrmzbx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gqwjengzh.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glogywnzy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtygrucl.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gaopnoxhb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gwxgxprlx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gvaylrlqo.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gzaztcgif.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gbpmcdoeb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/givnprxph.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/ghzzrpxnw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gdzruspva.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gytxkvppy.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gervpmgzv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/giqhrlnhd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gagdudlpf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gnkgoqypg.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gylwerejh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gwmgizeho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gphdaqlew.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gkxawywuc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/guzzzfpaa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gqnemjiuk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gfavxvfee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gengdmogd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gtdrffahw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gssqwjvof.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gvzoonsec.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gnjewtwaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gplfhpuct.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gjszsdabf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gwflcrhsf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gnyjsgqrv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwyamlbus.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gkdhkostf.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glqdfuthq.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpffshrdv.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gezbjmbes.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/glmxwjidb.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbhcpzljv.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gkyifroke.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbhotrjfk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gcgonjhke.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gcuskuurq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbonhiqdg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gwiwduijz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/goltgeufa.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/giwqcxedy.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gcozswqvm.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/ggqiyzqhl.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gnuyfesiw.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gabvpprav.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gorvyszek.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gqgwuouvn.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gfgygtpap.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/graxdctru.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gyfxymuyy.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gthkxipdf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gahshpxtk.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gkflrwxbi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gtdnzxgzg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gestfljfu.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gawxtjejz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gabuawwnx.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/girwofzox.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gfulyueok.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gwamhdcqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gnrvzmnsd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glybqtzue.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gkyzfisvf.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gbrshkuad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gdbzcnail.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/ggcxieocm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtkytscop.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvenwboad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gibtonxap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gluskjgqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gkojjqbft.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gjadbcvsc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gdnzyavas.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gbxkjramr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gupuiklhv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gxajisovk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/guecjbmqa.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gzvmxynqp.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gsphokbpj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gktdbvkeu.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gqwkqlduy.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gpkdkbhij.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gcdzdgckh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ggvjjbhqs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gssygaypo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gzmvzacam.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gervetfcc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gxasijqix.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdyyekp.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gspmbosxt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gnslkvfnr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gsjdwdbmp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gqohwcfzy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/godleaxty.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gmdttszrt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gjpywqjkk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gkoqiczgk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gnzubzkug.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gxgzlqomg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gumjjlgbu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gjfxoggfq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/glcjwfxvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnfqaalkp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/glmfesoro.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gkefevoti.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkvltnhls.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gogiribkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gaarscasm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjezygzjy.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gruugkyal.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gagxszkqf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gvxhnvqnj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gyfunkdhq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/glsudytez.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gvrdbarqg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gqlvpmjrj.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gfuzvbpbz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gzqsdkxpj.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gcftiflmc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gsojpqsgt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxcipanus.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyabycggo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gnbnoxzde.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gmyeeflbh.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gfddfufzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gbtcqkyny.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gppejvvxr.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gyyqicrxq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gecglyxse.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmaxtipcy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gntwhjbhx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gyvuokldx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/ginmmcifi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gziayhngm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gkksftapp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gvnciadxz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gaeskzqxc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gjncdewxq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gvbnrgzrj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gxjgisson.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/ghzppmptr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gxvtzpuag.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gnpfombrc.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gygunrftb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gohsplgmc.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gkafvumyq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gerrntabm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gvqxxzzkq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gmytvkgbf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gjfqgxmft.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gopcvzsrl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gnxzzwmgr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gbkkwmiwa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gtfrxwilm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gkzeuuree.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkvavugbe.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/ghcoravgx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glsfpmtqs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gjasrhdoy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/ggxpxhvhc.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gzraylpik.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfumzchnz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gjydcfemc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gihzxsivs.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gfcxjqmez.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gartafljw.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfxsokcwn.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggtgtboed.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gjaasnhjz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gutbmfxqv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gqpnnqeop.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/guujlmoib.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gbfqpvxas.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghfdoqcxs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gwfnwpfno.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gwciiatto.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gemhnawls.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/glxtgdalm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gnbwtdixo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gafctkulp.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gvlnqectb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/guylulbao.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnseokkxl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gvryamnfy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gicwxrael.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqpclytye.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gvlybsbwp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqcurahlr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gjxowqefv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gxcvpqxdx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gbqjokgxq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/giumfxzhj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gjtjbulyj.sHtML


<!-- 参考信息 -->