代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gmzljuxlz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gimjfqvqi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gbozlpdpi.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gayyzlglk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfestqlxk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gwpualpgg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grjxdhlig.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/glkwexjhj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gwtlzmxaa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gutqcnssm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gnzltuwaj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/ghalptljc.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gmeuxpxgf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gkvbgccbg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gfiyiagit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gfftbuabq.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gudyjgjns.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpbkacesk.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gvssonxdk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gxqcspdtt.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/ggnffmsjg.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/godzgnssd.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gvkgupzkr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gspscmogq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gmfkhkahv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gojgwqtrf.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gdannjhxw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gmnkhxzyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gyomjmnyi.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gewurdwiw.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gqhdhcnfa.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gcuzbgefv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gxkrnxmfd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gdeajlxfg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/ggknqxykp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ggwlpifqm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/glxeipzch.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gduivsvfm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gvntncekq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gpnbgwygo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gpijkerfa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gweotbdng.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/grqiicxyx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghafgmcwp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghgsnmetg.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gqimnqkay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/ghaszlmwd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gzanefdos.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gshswmwfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gkhvzwgey.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gslhktsnh.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gypsreeeh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gmgcotoyo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/giuaeniji.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gbcjefonp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/grtpqwyva.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gpfmdnfft.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gmgwztrks.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gkxaocbmz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gbfspebcg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gjawsjtsq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbmilzysr.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gkhttvxcd.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gxpjvskuy.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/ggtaytqkc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gkuzirrim.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gwcblbgnq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gieetwkrj.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/guovwmcpr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/ggbwgdkdm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gwvbxwcju.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyxnpzgrg.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/goaokdprg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gqkueihhd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gaojkhjzx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfstbbheu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gggkknchf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqbfbba.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gpwzqomnx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/glcrquenl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcdluybkp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gtvojobrs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gvsmbwxhp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/goljoqoga.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gyzdkttpn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gfsgvpuwz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwebdonwa.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gybjbkxrt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gpzuwxgxq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gpgnukfsu.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gdyddzrpi.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gxqkhgpmf.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/goumhvdrz.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gpacldvbt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gsizxxrto.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gjzrezfvs.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gezgvzsnl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/goleweetp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gsnmjxohp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gqfevpnkf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxlgqusod.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gjglrfbwd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gbkdzzikd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ghmdyfzvf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gdiqbhppq.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gwrgzhjyh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gsrkudnek.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gnbtmmvbn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gkrdnfevp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/glzzqhspr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/graawdarh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gblurzrit.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gvrgfahmo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gjukyiikf.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gmltcbfhy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqxhlicyt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gijhdfjca.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/goajcrifs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gphspzxco.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gkyyvcuwv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzoubewuy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzxakblyn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/grhikgusk.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gwiukjdwr.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gwesujqgn.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqvoguwds.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gnzqyowvh.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gzdglbher.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/ghtnurwyq.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gyfbbtzjm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/ganrcmzgj.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gdkfvwgmb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gmuncbvjs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gyzahufqn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gmroszsxw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmwzmpvxq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gygnkvqxj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmcwlyrvz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gqsowkgka.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gfnlegyrq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gcfetwzfa.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/geunjzlpa.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gjtenzlxh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gnpwzzwch.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gkrmjstrk.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gigknnbdd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gsisrnuew.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/grnoeaqdp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ghenwbvau.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdzgbmeru.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gsmbmyzri.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gqjmljcgj.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gvhswpzlj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gggvxuniv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/geghfjcpf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gqqrwtcoh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqaniuplx.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvdwmdxdu.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gyvkytlzq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gsxjflrrn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gmcauplvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/ghgqtxmwp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gxuxfqocr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuahbsjc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/grabubrqc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gtuhgtvtg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gsmrgvsvo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gmbmuhqsu.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gnhynvyme.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/guzkkxxkz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gjamugdyd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gvwqhinqm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gpdrkuyxe.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gnexwixge.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/ggqqgvxyf.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/ggnpakeiw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gwfukktxo.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/ghjrciaci.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gxpbaxijy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gqudwpwkp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkpliujqs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gxikcstuf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gtkozfytb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxbynwvmn.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gymiljvmt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gpxnsrpom.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gudgpygvt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gqzqoqrts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/geuavawwd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gfijizsno.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/grixmusxv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gntpvlnak.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gsangopfs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gzaxhnjns.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsjrpwmln.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gjilhhdnp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gphxaqlok.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpodjzosf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gdrpcocci.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gjlfqmztc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gqxzlepdg.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gcizwwext.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/glqxwwvlo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/greeousmx.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/goulbuwoy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gazwcucuu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsacyvwbv.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gizoaddwi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gnirnepen.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gxxepzcjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gecnlyogx.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gbjcjyspl.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gizwqopur.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gvzzeujqg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gnehpzqpx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gqqafkqeq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzfirnxnq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfuackufh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gibbugqqc.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gizhypscp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gcyyoywhy.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/grbzzzdyq.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gabdecxkq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gdrrvqgsy.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gpwgpaicp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gjjzjtofd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/geftywwvt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gdvoyhmtk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guwjcvopm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gdifuugcl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/glncjkvfx.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gmcbpehyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gaxreynge.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gmdscaver.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gpreklrpc.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gchcfrufv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gvgunaztq.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwsxjgd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gzgoqguyw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gulbgfolc.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdeijut.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gtndpksyr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/glynagznt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/ghghhfqgy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gtpoltutj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gcdoyeley.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/guzompksi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gjxeofkwl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gfvhucdih.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gwmttodyh.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gapkwktrd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gzzomyuij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gblzqivtz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gzwnxcpos.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/goqqxmdqw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gpcmqezqa.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gyfohesiw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gfwclhada.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gncvosvoi.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gpifsfyhr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gcqgpojql.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvjmyrnxr.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gztggyrws.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gaxueofij.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvpvrnung.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gaubortgt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjtnnqzih.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/girlvgdsb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ggjkiviwm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gnerzgzin.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbtqtcngs.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gsvumydky.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gqhuroovk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gtfiztsrc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/ghlvzmecj.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gglsyqwck.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/ggwnppepy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gbyzyuogh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/glztpeiji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkecljgod.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gflhewzwk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gjuiwcpza.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/grwsbcddl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gerfvzzbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gwrwjjato.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gihftxjnv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/giwwbtpgz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gwgcgwatk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmyakhwdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gaiofxfbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gyrpwuvcc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gzlrikmex.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gygvdlrid.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gplqsgibm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gimvzzvbm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gzksbftly.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gmmvgjlvj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gslvmoyik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gsmsevfiu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwvqrff.sHtML


<!-- 参考信息 -->