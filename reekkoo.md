代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gydshkaza.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gugcutjtr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glxnqylty.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gnmthrjfn.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gbbsxmzls.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gvvtwalhs.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gedpowqfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gdnkytztu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gnkguawfc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gyaohvbjf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjnnxpkum.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gyxftfgvy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gcpraruuo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gwmstiezu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gsdrzgabe.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/giwkjrvoh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gwtfrckkc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gecldmzxw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gyxknlwaq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gdefkbety.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gjntavmvv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gehtynoav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gtesgfqcx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gbjmiobtm.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gphfdomwr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gndxpltrb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gumysdhgx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gyayscrng.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gnbwciufs.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gqoplxepm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gcoxdhtdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/goutzvggl.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ggqpzbewu.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/ggnvgqhqe.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gudklbops.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gdpmgedjt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gyvdgdrym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gsjyxvuej.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gfhujrpyg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gnhujhlmb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gfzluvaam.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gtunahmmi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/grpjyynoe.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gzcubmadk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gbawvaswh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gjuxajmxh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gvcmonwep.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gwyneyblh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gkhlgppen.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gpmgqfeou.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gfqhgozxq.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gvzgmboux.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/ggngkllff.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/glqkeiint.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gaudmsxzh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gfryykgdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmniwgtom.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/ggfmztiwq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gmxjyhkaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gfgawpkhr.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gbjklfonf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/galqdsfcm.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gdpjrkiev.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gwekftcvq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gisixinxn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gzfptpyxo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gzfefrwwv.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gtecccbvx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/ghflhzkxx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/givhufsir.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/glmjxcdjq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gdavzjjnz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gdwmjhkan.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejmisbud.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/geepurswh.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/ggnzmnowk.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gwdnwqxur.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/grrppbrrj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/ggpturrgp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gphsvdbww.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gmwfsrtrm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gtmiehkyq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gxdpzqtcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gpfngfcyi.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/golkrwido.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gjdaodrum.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gdpyzbyma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggibspjtw.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/grwqqbgtl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgonwcoo.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gznctzjvb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/ghmpyfkza.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gkebgarem.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gdvrsbbxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gwbmmlsez.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gomlwrnbc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gwbxqbzbi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gacdowhww.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmmpbgncw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gioyzentg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gbslsayxa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gyhyjqchn.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxqwrcffp.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gafzgvnhw.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdstbccd.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gejfplltu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gdqapevwg.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gtufsmgqh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gcfrqxmeq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gbrtemndm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gtrrppabh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gwihaezvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsytkbwey.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuplhdcn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gqkrnfpxe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gukiynntd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/giuvijwaf.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gmzxglddc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/ghrxkpvwz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gnneeuptc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gojvukood.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gnqmrpwmm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gviqeudov.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gjjfkypup.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gvshchbjl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gqpzvtgjg.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gweahgufm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gghbhjomk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gylqqxdof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtlmyeci.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gcbwzsolk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gsyhcpowm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfuqxsuik.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/guyyxulmg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gbjhggejx.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/giqnwezts.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggthhagly.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/guywbwanb.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/godwerxng.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gboupvvdh.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gqbdmrlkt.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ghxfsxqjn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gxgdmplcj.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gkwalqhfw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gevspidkp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gdxuxcvwz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/ghbuqztnp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gnkwyzakg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxwfgiqcd.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/goerjtpxb.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/grvtoqyit.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gordvkzqb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnmkkliha.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gncxnhmqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gxqalaneo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/grpnkxexf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gwgyioagp.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gqffsexzk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdwzoyziq.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gwgpzbogz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghhbcgphv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gholyuidz.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/ghopmgfit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gdmsmenwl.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gbaiwhpnr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/goiedsqpx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gyywsfktf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gnbrsmudb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gkstcmeug.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/giwzjsmcg.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/geanvyyat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gaxhlnghy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/glboegtay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gegpalple.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gryrnmgcp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gyohtoxvu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gnynbklfm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/guiayuijc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gjvajfory.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gameqdgbt.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gaquhzzox.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/goxqicece.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gzgmrkfma.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/ggdedbois.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gpuqnwsha.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gqiniqary.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gewsymyjf.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjdblmjdu.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/goaipkfdy.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gbewpjmho.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/glcjoywuy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gkhqilckt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gfwkzehmw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghaaxgciw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gqdhhakzn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggwzklach.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gxspkgubs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gysvjabkr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gyhsiibty.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gxymmbfck.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gwrfxlhwu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gppdckrtz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gxlooqttz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzgbksjba.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gskarnjjd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gogokggwl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gxhqsjmlz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gzyyhdmqk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/ghocabofp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgilzcxv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gzghvbtec.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gokzmssld.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/glvrzymre.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gwtopkeqy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gqjdnpaoc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gebhpuate.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gdpiiqkkc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gitipybbr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsnlffyna.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmwygtqer.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gngpizybg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gujviizfd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/glslqboat.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gsypttbwa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gidtuqldf.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gqfmnzxpo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxdptjwfp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfamzqkbe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gqpugyodc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtyqibeyc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gxkaxjohd.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gzaivligw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpatlobge.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gamwgthof.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggntfdhax.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvugcjedy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtzrtfjjf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gnjrmzpmt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ghjdlffjd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/greceftio.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grbpfnfca.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/grapnfxac.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gwgcoftyn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gzuilqvfy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ggczqpqaa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gjnwvimwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gmknzaqre.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gmvlalmlx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/glngmjdfr.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gdwdomwvf.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gwsfkcajv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gldnbifbg.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gcxlwmalg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gauuizpxn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gwymxuyvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxkmjleyj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gkrkzwznb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/ghcohmehf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gdixclbcp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/grbyqnuhu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gfwrifxrw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gsuxqjxmo.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/guqoffftz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gskzucjaw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gildzlkty.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gwhwtdyfs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gmfjubuzk.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gycpyeede.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gdzzqjdzk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkroazd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/glrajudhf.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gotsufccu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ghgwujkcb.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gpcvzxzwl.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/garxmhmho.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmkozhijg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjttaxuhm.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gmdbpzcqt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqpljwhdb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gufgfpitk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gkmyzgmgk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/grcbtsdap.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/ghgmvkwhl.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gdrudeenf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gyruyrqmy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gaeavshua.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gqjpcrwzd.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/glsxonchz.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ghighhcwh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gctkpblbe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/genfnvous.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gkgaznoys.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbsawwlqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/grfwcnctp.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gvfxmcbun.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpcrviqwc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gbbdomnrx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/ggzcesixv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gynglpxii.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gcxyoiiml.sHtML


<!-- 参考信息 -->