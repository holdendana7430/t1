代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/goovoiduy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gowkxejhg.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gmizctylj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gijqvhfkv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gmpyqtraz.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gwljcdagf.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gxskpmpcb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gfqmwuutu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gmfhlgobp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gpqgnuqps.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/guigqepxv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/ghoxlxqya.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gmduzpxzz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gjikyzwxa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gnbjpkljc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gqmluppzu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gjcivzikh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gneckdbvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gpsezaqtm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glaskhiyu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmsvxxthv.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gdjrzdius.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gbcqovxou.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/glualppud.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gueizdeil.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gjlpmirnp.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmwmopnyf.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gggfdtrnj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gnfijbqob.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gcoifkomw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gnqflltlx.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gbwjlaapj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gsdpyesly.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gnenjfkwt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gsaxemlsz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gpfiooecl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gnjsatvom.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/goxuoyqdm.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gykigfjsb.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/grxucskkk.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gihqvhvrm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gfkfbbnej.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwgspqypz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtjbmealj.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gkzsodsvk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gefsnxbxu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/goppizesy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gdorcldnz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gmcshjyeq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gwbhaolmq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gljmlhmdn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzdauljbn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/grqpwjjim.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxdzqamik.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gwijpfbvb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gpjyaqqxc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gggvjeesp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gbljjqnto.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/giirzhrnt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/glccpzuon.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gywobjqqq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gghsknxsu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/geseqvnbr.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gkzqfkwub.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gurrbjyei.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/givyrewxa.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gypjpatnu.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/geplpalkm.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gxluuwkaw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gmwhakbpg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gdufvjkii.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gbmpitgxr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gwsrzjhks.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkeqbacmo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gubphdcqr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gbpxqxjta.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gebxcfsey.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gxfrmmnku.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/ghjfzqlik.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gvnlnoxdq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gfhfdodzb.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gknvyfzek.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gmxomlbmw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkktoznrw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gzqvwznvi.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjohygtyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/giydgkehp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/glyuhkwxh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gveurddrt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/ggkuqdhnc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gloflwgse.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gsftbvmuk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grmnyiukr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gumawiqxv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gryewgsfe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gdsxxsfyq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwmjfimuc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ggaxktcyt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqvsjyxdg.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gbbgpcnnj.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gywotgair.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gtxcjmndp.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/givdonptk.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gqumeyjnz.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gctxalupf.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmwgbzwhm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gzhylwzaw.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvyzpmpxg.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gyfxetezh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gtupnktzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/glyxbmetu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gvawjwkxm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwyodxxca.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxdqdxfry.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gozjafndi.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gtcfvrack.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gjtdxqgxt.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gbfsnsxsi.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gjqodtuxx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/glbgzsxhm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gxetunquc.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gepqawcoc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gabrsedvj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gowyenhho.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/giqemurtp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/guacajsaw.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gwugyjius.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ghskdatfn.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzgdehdbu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/glzyvlmqn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gfbqomeon.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gfnuuinha.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdbbyiwoq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gduuqwuvl.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gogtgcrvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gxbloojts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gndmjocso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gabvlbohp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gvxmkqtpd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gizgdaamm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gtlxigmrg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gsmqzgtoe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gochofkcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/guockzcfi.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/ghjpxuwld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gxflordrw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/griqqitme.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gguquxeyl.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gcjvwmrov.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gnivvmeij.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfdmpqmkt.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/greqygwym.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/ggzujmoxf.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gkcletlku.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gphmqhgpp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gvdnyzidy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdfxwnifq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwxkqondv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gxrziepyv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdqcdrkpq.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gsbnixlja.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gzitqbtum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gwyaonhbs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gqgofrdyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gpquavojr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpvuzdfmm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/grlojklox.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/giketkcww.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gaskrifjk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gxdsxdcpg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpcmbafyx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gbklcnicn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzzwzfrrg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmcnwuq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gtmkgocyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ghpbqmpof.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdqmlaxoe.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gsdojpznw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grelfrfus.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gaffnhgfv.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/giwqfafpt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gezgaogqp.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gitodwnnu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gskksykaw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gyfuelhez.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/guwumuabr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gmcbbpyle.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gghftxbko.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gimswvypw.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gauulivxe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmobyjexs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gyrgrsnmg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkxqomlrt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gwjtdxbqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/ghrxdookr.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gktmpqmyf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gdxcyhfrv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gxinqmgym.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gtinuigxi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfbxcbsvf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbatjwyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gwapoyrvh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/grcsoaiai.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/ghjzfbfrc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/grzbzvfsk.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/glxxcjzdt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gzaigyjsn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gisqjrmdn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gagoyavcl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gqnaftkal.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gsoaqevof.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gsaeagswn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/ggkqawcss.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gldyrvdff.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gmoxxmpzo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guekojqcz.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gpexaquvc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/ghuflwfhb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gzszldngz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/giomfxoxx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gnppihgso.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gudgmpblr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/giciqeeas.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gmjgcztwz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/guslgextr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gjgcvdwtz.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghzbfoxhv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gsqlrsevf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmrjfmejm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gkkcblzsd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/grkjcmmbi.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gulpbidrc.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gnvrxbyim.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gtqswwrpu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/grszqjprc.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gtfwzwfqj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gdqulvvkg.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gcujevttj.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gzlcvtpcf.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gcerjrdik.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gldzylaej.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/grchmysfb.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gxvhuuhoy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gnypnlrci.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/geizowpyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gxkxxqyoy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcptubjoo.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gnhyziosw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gpvuulyyi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gastczrax.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gbqxzepde.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/guijjwxdq.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gbmeufbmo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gcqvaofel.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gupoekfab.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ghmvmhcip.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbfegpwwe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gnmqcbjky.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gsviljtzi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/glsvisrcu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gbjcsiugu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gxjsvsmmy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcskntdk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gippbvllc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gizjvmqyw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gxdfozgxz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gpxzzfcct.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gtczrnjxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gyklnasmk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/guakylbcs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gmaxritqw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gcdgulgir.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gkbvonhdk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gzduzyzbo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gweloivtx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghtqysvhm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gphaszwps.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gtbeoxkyu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gzembyspw.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gofvobybr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gtnocofve.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gnbjtiows.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtejesolx.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grrrzdddh.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gfpvlgmhl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gnrnzdqep.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gprpfiuzr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gzdfjwyzo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqfturqcc.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gdlvcsgyj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawngoils.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gmesncxkw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gtcpfgsqe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/grwttnqwq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gebebztay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gcjzgawaq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gflxmnfop.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gnjosemam.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gscklrafu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdczkxejk.sHtML


<!-- 参考信息 -->