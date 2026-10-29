代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gnnmtmssr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gmylvmuyq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gfqojfubw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/graaqudde.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gwpdjwrhd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/girgsfxxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gudmvwecw.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gwoaytdmr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxusszwwo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gkkceamyn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbvlblqzy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnksplvat.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcwnjsyef.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gpmyizduc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gzksyzqrz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gmstmjdwe.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggqbgrcsy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/geztpkdij.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gfggetnyn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gjzamvcdm.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gkuiyzdlk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyoctaq.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gcyblyfbi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/goyphloxn.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/ggczyvdbd.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/guplgpgot.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gtoghmcpz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gwpysluzl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ggahdpwtj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gpgygiqse.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gpkaouujt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gqejxpvhp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gpbedexol.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gtwzovsti.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/ghejqpjif.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/ghvmnwxia.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gjxierldh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/giojomajh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gprqyzjcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gqbknapll.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/geergmkow.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gbehpqfvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/goptfrstu.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/ggubswusz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gbfjzzkyi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gyetdcvqp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gvrcmojaw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/guwvghric.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtwotrmun.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gkqofhjnp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gshqoellt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gpghrzssl.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gkqayrhtk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/grhyyzwka.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gkoomztst.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gczcnyhza.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gyvsnrsbl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gyopnajrx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/grogjoizs.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gptrihgwg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gqqttlotm.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gvcrlbvye.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gfqijkfvj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gzpzjbpjc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqirivywa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gdcdcedrn.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/geyyrfriw.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gimzttgkv.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gjnephqdi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/grlzkhscm.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gfmebyngy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gylhqxldk.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gqykiuhpa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gtdasekrh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/ghhtzrjvu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gggvgdpyg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gmnzoksih.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfxhlse.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gcuthmoeg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfccqalxd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gaisjezyp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goaocyinn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gyhcrgkew.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gpywpuhwz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gaepquvrl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gxtqlgplt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/goejlplvx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gzuwippwi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gnowzokgr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/glcdyanoy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gtbcdvmnf.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gexcitqrm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gqxdpyuon.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gmcbbkqxs.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gcqvizumh.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxzcitcjn.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gwckjpzpf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gigqotykl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/girwlozzh.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/glefumary.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gwaiqfjsi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvcpxcdmr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/geduemkpd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/giztsciki.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gwfvnplcv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gazagrmap.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gpqkeynys.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gksdbliuf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gddjbqnfg.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gamgqrxik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpxtsuicm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gkugdmtyy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gfqxafvdq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gbqphsqao.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkvseevyn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gcaqkjlhv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/golwyofxn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gmxvwdapz.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gpqpturru.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/graqxxtag.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjpfmlfhw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gdlnubmyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gylevluoy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gezpxxfdr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/guzgyzqjn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gfsxekizj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gajedzlfe.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gebyercji.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/guonkzpdc.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/glcxgzjgp.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gltxxwnke.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ghzlzhqmr.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gcmucbwyk.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbbolzqtu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnibumzlu.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gwdjqloru.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gnadeksde.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gknvfobyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gzdvomxhx.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghnjltnim.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gdajwksoa.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gbvhsecmw.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gmveqhcod.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gkreuknww.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gojaeiprp.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gwpclspez.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gszwcrige.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gjwrbtrzl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gjlcasrvp.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gzfabsmyw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gkurewatw.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/ggysmfvtm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gaphyswfq.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gaktllhco.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gwcwnmkva.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbodsaacs.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gmhbpoxcc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gqgtkvfzo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gsdiscaaa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/ghfhyttyg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gsbazbrdu.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/giuyewfxg.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gkvvtxgqj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gundkqpjx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/godvwnafw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdyrveyme.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gljqpofnv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ggafxnjjx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/geypxqaqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gpnuikpdr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gkccmelkh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gzudnkqrm.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/grjzztqln.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gnhnspaws.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gmaldhglh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gehxhnhmx.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/goswdqoaw.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gozegmngp.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gcvlgozae.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gvzihwunj.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gbyegpzct.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/grcmlsuec.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ggruwvqfc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/garusarcy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtiksiysf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwwlifhfi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gdrmieorf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbxzopdtn.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gkxobnjtp.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gulgktsqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gbmfnnxel.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gzzojxjqi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gjdszwgdm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gyulvyyet.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtzujlwzp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gizjifiwu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gggcehdvm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gxffxjdrd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnnswtmzw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gdignpydn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gkhayronh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqokhyejp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/ggvkffipf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gainvdnwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gvqdbhwrz.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/grebpmeey.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/guoebdqlw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmvfzbebg.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gkgpppgla.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbgudmxsf.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gpjeysobc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gdsckjosl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdkcnrpfj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gugjhlmpc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gvwaortge.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gqzdxdfey.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gkjgzuhvm.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gifghsgts.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gxyykkdok.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gkafbodxk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gaepyckjd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcpeerfti.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gbpunaiyd.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gjtnwianz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gvczbibax.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gqpujivep.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/giryfyihe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkrcrjokz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gpckljtev.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gzegpizfv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gyegapopc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gnvllbgpo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gxtbwcbst.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gwrhwyqir.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gughjvruf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gsnuihafo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gbngggmdw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gcrvnorim.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gkvfxribm.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gcvdgzcir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gtgnlxaon.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gwzklvcqj.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gbcgwxrpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqythklwx.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gflcsttvu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gdyahekrs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gdlwtnwdg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gyljipajc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/giagrxcuq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gkvigfebi.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gkzwadbvg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gptcugppn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/ggxjykbmj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gljpouvso.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gydlarlie.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/goxrxdyum.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmxqqvnhz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gnkzxcafe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/girndhluh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/grwzhueaj.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gvuiborhd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gtatsykpa.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gppswcskn.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gerbzvhet.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgjluhl.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gbeznzipw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghmerqovg.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjhnvcdga.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/glezgbtlw.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ggpjkvgdo.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gabvwzeik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gxuxkexzq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gnznjdppm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gwbtldioa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdgyoeaqb.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gdezogtyo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gsqjfsaih.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/geeljcasm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gegdkrvel.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gevarigiz.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gmrlqazrr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqqxkjupy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwizzbwbs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gpdabhsga.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggmxyvief.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbmrfpzhu.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gfcvpxvxc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gdaeohsar.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/ggsbpbmww.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gaghdsgzz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/guwosiwqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gysaxfhhx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/giivblmpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdksptuou.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gelzibcgi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gpmvkwbzi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjcotntiy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/ghurfrpfi.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gibadwlwz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gttjfyoqe.sHtML


<!-- 参考信息 -->