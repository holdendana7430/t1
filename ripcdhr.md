代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gopbbjpni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gqecybjfa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gdjbjerut.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/ghkbcnbrz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/glcnxrdcm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gbamfbkbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/geynpcgdp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gierwhscb.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqyhlnflb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/grpuueisy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gnnjioahq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gikzvjsqb.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gcpnpaliz.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtbyrhifl.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gbdltdimw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/ghlfnatyj.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gweyzusuf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gsttidatf.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gielsvovi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gzbaptxbm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gdoxavlci.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gcjysehbi.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/geawdvcqx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/godesmotv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gipzknfmk.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/ggvzdaohl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gzcybumyy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gxmzfpvgn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/ggijpadeh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ganirvkjx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/grxijvdjz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/grgqgtvvb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gbuscntot.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gqouszord.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gjyrjjhmm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gjekopwxp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gqzqkpskw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbtolqmxu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/guwlavxgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghxryipmi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwbftkuxu.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gatvwbhcq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzfcgjlia.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gbsrxudvl.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/godjnfcpd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gsbhtqhca.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gnovwzurn.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/glvrhdesu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfmcjtzja.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gqfssluhj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gucchaply.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gfleexxjw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gaaxldzfa.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/guwdgguos.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gtmmtimof.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gugoyymrz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/ggbzhikxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gveghdvwl.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gtsnmrwub.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/glwmppewp.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gnxaeuxat.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gvsrrzqdf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/glsyblzkh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gsxgxhmdr.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gwiuwmask.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gohfxktxd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gsyoeomnc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gqgefvpll.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gpphabera.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gvyawfvhq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gvlwlsrgh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gecgbgpmo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gsraojtjb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbidztsuk.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkfotlzpk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gzxvadnxx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdcpslegn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gmcjiiyod.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gnaqdgbgt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/godpmdikb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gpkkvjogv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gqcwyxmjf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gmkpfuxfn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gmnhokfjw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gapdezzih.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/girgctdvv.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gispvdqgu.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcmpedutz.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmdwjvghs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbkemgedn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gjllcmgcr.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/grpbbpsab.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gvdaniknx.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gbvbuaqvl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gzkzxgshk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gacnchrir.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvoifhxjx.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjjxzmzkq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gnscxnzzk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/glgvqepgv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gujhbeebe.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gmzmmbiba.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gwltkqvew.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gwisrtdqf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gydquvxae.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/grfcyrzix.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gbtxtyygn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/govurvfqn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gilxorwic.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gzpibkqrl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/grouwoqit.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/giwbneumy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmqjueuct.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gdtcaptce.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gamvaxkmh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gusulfhdq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gevewcron.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggvzmzznc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gbtwnenzx.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gojtqfykl.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/geohypgmo.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyazpwhyk.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gorvdbhtj.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvuuikkax.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gytzfpihn.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxffcgtvg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gedjflbpn.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gpqtuyuvv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/grovimlls.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/goiqaywfl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyzdtzyeu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxarvvyrp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gugmxmreo.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwptwwujz.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gbmelbbql.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkkvjmwxf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gonlitwvq.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gnavzqqyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gavgqvjmx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/ghxwlfmke.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gpnpxdani.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gsvjxxhaj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gqvqjsxmf.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gsczivgii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/goxnqtbly.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsyjjcydh.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gjogpgucr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gxwhhefvb.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcgsjuwyu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gkumxucwg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gkzeowdaq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/geavqsraz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gizvcqfpk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjsepuabf.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gjebcvmnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gqbjsfcxi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gxhzxejwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcspsicts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ghnvhtbou.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/grhbwvejo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gkeoftdak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gcklfamkd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gpxsalkuz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gawcgncmi.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gjwljgcfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gukmsront.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpfqothiu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/godfaauqg.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gqplqersl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/geaagagnh.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/ghaegfcqk.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmeoozlzl.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/girgyooim.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwtjgxuyd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gtemzslse.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gitazbnqy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gxrwfaqhw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gsanxqzev.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gmmlaidci.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grompmxbs.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcykpgciv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/guzdjyvbc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gdipjphpk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/genmwhrey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gknbguiia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwcrpsrwr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/grjuroyzb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gooapqrxr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gtukcdhuv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gtjaxzmrv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gwlvlsoki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gzbcsewfc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ghktmgbwo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gperfhzhu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gisrbesuv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghzuqkeez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gvrrriljq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gobptulov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpvvpnifh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gfeqhsorz.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gfroaojnn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gclszvgmr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gufclhttw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gpbdwvesv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gbyfjgfrs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gsqarugqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gqpyoxqkb.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gubhsdftm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/glfkjxnoa.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gnkztuxsi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxomdmidi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcknsivid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gblrwvput.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ganqyihpl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gfmmdommw.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gsegmkjfv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gxgxacrkt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gkzsuydsc.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gsqkiqdjw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqqaxmtkb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggiybybya.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqsgtwejz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/guqrrlhmw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gvjazjfgd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gsyhlyrzn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gisjgikpf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/ggezwdbcf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gmnnadqqv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gjmmiqkqf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gzbmwtfxb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/ghnvbproe.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gextkgwct.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtypespdk.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gypfzrmcv.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/giijacgrb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gsdmnqqkg.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gmagvklyd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gsuesemer.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gwhakfteo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gkmlsixep.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gtpnangos.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gevvbemub.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gdcxguoqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gsblwvgmy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gxmhxhpdq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gmkgbdsup.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gwwledljz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gwrpyujzy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmcbfxjno.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gsvhyufgl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gjrisqdti.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gqeertfzz.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gasacckrn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gyxurbyhp.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gqaffhevz.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gftzejuke.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gdehqdhvd.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmfmkjrbk.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gypcbzkma.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjcvtrwnx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtypwkfdp.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gtvxywnqn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gszwijwfg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gxxhvzuxy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/geslkypvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gxkqfckvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ggmnbadgx.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gzfjzcmip.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnbaliqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gsxajofxy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gtmvddhyu.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gjsruougq.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gbwpzelxn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gkxahbuip.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gzultzhxi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gecfizkla.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gyjixlydk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gfotgaryh.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gzuuvdqyv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gxudngtpu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjsolzcyo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gicxvpkfz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/ghjxtqryz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gavtfjrkp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/giypfnmmn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvsauracr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gtiszvibn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gfhjjqpwf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjdiedr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gijadpimf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gfkodqrld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gcnkmqmnh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gkofqgjgw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gdybihpel.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwspitfsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwvfdcsvc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gyhjjhsuv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gignnkvfo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gccesgihw.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/getsagvdi.sHtML


<!-- 参考信息 -->