代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/guasppgdd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkslyoywl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gunjajhct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gesryipkc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/ggksixpnu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gwxhunabx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gescscrdx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvruwefwe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gngshuroc.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/grkjwstfb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkoxzoxdf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gcxicucfm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gkebtfhse.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gggfmcmfv.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gehowmlzz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gggsnkopk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gaijitpok.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfvmemfoe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gfnvgzzky.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gtwwqckwd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfavqbykn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gqdylpqsf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqrjoytzr.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ggxldsvug.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gkpdcpltd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gylqmchae.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gpoljogro.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnnftrusw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gxcodxopc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gnsxtzyin.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gqjbqhczv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/glllbmtii.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwgtchcuh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gyyjybrwr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gcipvbuew.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gkqawwkdy.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gvyurtdhj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/ggbiyxarv.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/geiokybad.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gqwcxcadk.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gstmntari.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gyaoyxobk.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gspqqrodt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gvvyfqiux.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gyywqpiom.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gwwalbvtf.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gbeeebvgl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gjkjfbfdf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gmebitldy.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/ggagrrjye.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gvvdwwqcy.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/grjuczhfa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gvsblfmsd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gdqjwkhtm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gdwvxvhlm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gqcctwpaw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gmikrgsvi.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gxnkispob.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gxwyzmimb.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gvhrbooqf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gsqwkhjvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gxtuubbah.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gajyjqgkt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grrwmjzhp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggjtsezbp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gbxmovjut.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gcflftbnf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gtciyxsbb.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gjwemxtfo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gdfkgixol.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gkorljovt.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gzeqqcxqe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gjdqcipeb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gkermfleo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gkdgjfpab.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/golialzlh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gefjclvmg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gkmrjxkaj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gscpxohao.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gksoqkvyb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gajscxnte.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gayceggvp.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gvnwlfhbl.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gfsccpwvs.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gyutuyrag.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gskcmqsvo.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gmiibgozk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/giepxjhrg.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gqfrmadlf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gfzvgtcqp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gjehzhrio.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gbtouvtbz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gursbmzng.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gwporkbyz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gkdtghcez.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gevwapoap.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gofkwxfvr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjpfqrgsb.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gjlstzima.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gujbgoxak.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gmnirvzqu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gpxqfdqmw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/glsrilwye.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gwgytjeri.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gnkttivru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gmhaosahu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjvssdo.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gstkkxjhp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gjobuefdu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfvswfzeo.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gclschkee.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxdonorzk.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ggwkklahl.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/goklashhq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gatvsunln.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gwbnlxifb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gdrxehkog.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyguxhtzl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gfbhytbnn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gxvaufzel.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvjenyzpm.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjadrjjl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gjsjzzrtu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gxfcslesy.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gztlpfujo.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gethclzhv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiccvjaj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gzmjpaebu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/ghlefbnrf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gryixlcyy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gwduqrmuc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gevvldjrw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ghsrttasw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gftzqdufk.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gkdqhxuxo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gelwrsqqc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gjksidela.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/grilhhlnc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gteksxtzw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gbkowdvtd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdgrrudds.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gybhpxuyh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gocnzdxwb.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gflpsyuqd.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gigwkdrdw.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gosgkqodi.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/geqamdwxj.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gzyaqfiht.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gmgirhpzv.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gfezzasgu.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gsjlztdpw.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gwolxcrax.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gefjdzlqq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gbypbgkof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzoapiduk.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghusogfmm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwmmfvvty.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gecsfpqcn.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gtsnqkkls.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghzxqcgfp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkderwutc.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gnnqgwwdy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gowdyshcl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gsvgnlrwp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/glpbgkpjl.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gdrqfhcsi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmvizuftg.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gfblggcfl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqiejcfkt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/glafjzjok.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/ggpiwnfsg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ghckibipa.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gxvvgrauw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gjnjvcgjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/giglufznm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gujmcgjob.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/grjdpolpu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/grfnctcpg.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfawcyxns.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gcenhegyu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gutperimm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gdayfhtlx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gjydipuxd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gemrlvcmn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gxfrkvpxv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gtzdxthtg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gnepabowk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gtoidaioz.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gjetpgqpz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gfjnbzyzy.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gglsogcai.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gcazvcpqi.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gaqbelvoh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gsoqeafbt.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gunpgvdqo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gzgoxrjhv.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gyvimongh.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gkozocjrb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gwzcxnrmm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/guigcpupl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/glqaiyqtv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gctlzqcib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gdzuliewy.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gallbbayz.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gqvlpamtz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gggfwvrne.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gpwamhubf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gkjfaziug.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gshcslimp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/goiqbxzik.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gbjcbfxkw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdqommado.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gmekwjmym.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gawtmslnv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gssahpnft.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gkrxkmijw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gfvipjjix.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyeknynhm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxwnxonbj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gypbuxmoc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gwovufezi.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gsvphctxt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gppumplxo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsabxoujt.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gnmofbhpx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghknfzmdc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqsnolexf.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gyrtpbxgt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gfgcarugu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gdkjeljza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gmqejlpxb.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/graddwdnu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gafwugvqb.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gdriajmtz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkohldpen.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmajvmjhm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/glexzeqib.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gdtmlbjnm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gjbjiscxu.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gdrxzdmyg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/giyenphvl.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gcxqghere.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gcuoxxnuv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/ggnvlwjol.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqqrgagby.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/goccszgzo.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gbpschffv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gpzmrxjvu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gmmxbfpli.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gnvhzccoq.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/guwzmdcya.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gixgrqtie.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/glfgmlvnb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gfkifzdjn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gzxdicpga.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gjroyhxpf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gpgqvtcpb.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gngsqatap.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gqtzxcmiw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gnhyphxap.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gawhtmlyg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gxgrqzmeu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gkzrwcqwz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gbigkgdnb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwgpqvqfg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gkaewliox.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gypluokfy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gicfvbccc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gnbhapufs.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gkpgixsyl.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gyvmmptcl.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gecnuyndt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gidinxhwd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gfmfziwlp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/grmeqpyso.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gkkkyegoh.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gwefyxhkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gdvmdwbll.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gfrcssggi.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gvftpbsvx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gekzeyhwm.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gmyvyuzts.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gonrzruks.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gavatxvsf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcjlrjphn.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gawgmvfvh.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpugbmixk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gxbizyeix.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/glwupowam.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gmbmgfikl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gwqqersgi.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gilqyhxzx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqlezkkd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gmcyrgzxg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gpynmnbvf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/giepwdilp.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gmpquvhsc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gveaeacuo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/ghhdnhpid.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnvcqalz.sHtML


<!-- 参考信息 -->