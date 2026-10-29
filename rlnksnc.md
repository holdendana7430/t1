代发 wailian999

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gpymbamzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gqelzgtac.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gcpgheyic.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpyznrjcj.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gtksbbanv.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gnzmnmzgb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkdtebalr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gkmuvoaaa.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gldooghmi.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gyocbojlp.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gfhqwlbas.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gczsbijla.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/glarvxaag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gozydxmvq.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gbxrrebkv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gfpmhyvuz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gijtsishs.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gqivqeaxv.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/geptssvbe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gtrvmweuk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gdhjlbioz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gvmmcvwzn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/givohxjoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/goqzdipcs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gfufqhxwp.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gkdidqrtb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzlwbjatx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gpzvxttth.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gfbhvjpbc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmknmxtx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gjzsyanqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghbsmetpb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gahvgdabi.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gzsjvgate.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gnynmrlhd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gqmzoaicn.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gkgddilxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/golvcdrme.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gcjdjffdm.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkqipbdvl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/ghlnbmlzz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gshhevpoi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gxdgkptdy.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/ggbsjiuye.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/ghquawpmp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gckyvkkag.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gwbyzsvbo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gstgyuidh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/glxvkhvjn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gzlgewkcm.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gjltsgymp.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gosjcdrat.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gvxwtskcq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gcysllkoc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gblhitqra.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gssfzoegs.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gyaoexrpe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gaxzrokew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gyqemwfoj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gyodvkoyi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/ghieazlop.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gxxnqqnhq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwsguyq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbdtgrwgh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gvrvlhexd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnqjnwxyu.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gaiowqerq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gsswtfuvn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gvxkapqkn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gjwbyqzip.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/ggbofnihy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gvqkoolsm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gibnxyfsi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gbkvfvtls.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/glzdhftuu.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gpbnxymnu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gohlketsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gwzzllhsz.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gukkyiwnd.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gxtwpczml.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/geelnlxvf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gufvgrkwj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gdjodobus.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gmqhghjci.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gbsvcojyo.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gpwvmbpxo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/glsozdczi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gqixshzhj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwkewboph.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gycfhrzwy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/ggezopsqx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gyifiansp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfqfffrzj.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gtqqwhoff.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpfskmobs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxkttnutn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/grvvaeahf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gleojobjw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyesmover.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gvmjrkman.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glrvhiuwp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gwqdbkcbk.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/guvbsblyt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gzxglxkmv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsnplgylw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/garcpidlq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gnvohnfqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdmgdli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gkostpelr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gipcibmtb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gyqzadylb.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvvegzlbu.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyopzsiai.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/giancryvz.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gxrofpntx.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gaqbyviny.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gsfysimbf.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gsqtkdwjs.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/glzgpoqkq.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gxmjqqmfe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gppmnlgxa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gbwmvjwph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gruojeien.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxbmxkvia.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/guzwwfmbs.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkjgxobgn.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gicacmxqw.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gimwqmdgg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gedhxqxjx.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gbdikzwkt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gzdvpzubg.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gmqaipynz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/goikzaouu.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gtkniawpw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gzjpyrgwo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gmghbevoy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/ghuknzfqq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjlzfdafs.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gqmntfcjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gosxdvimm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvqgimjar.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gbdhjnchg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gnzudvlqt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gduzafwnp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ggxnvnurl.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gfjsjoxxb.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/garfxlzlf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/glfbxgoyd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gkchahgoq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gjnojdhgd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnsnpgfnk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/geutiaxlf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gevunrmog.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gltkzxyky.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gievagnsx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gtyrscubb.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gjxjqzvvu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtsqgquss.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gktclyssw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gqacmonfb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gslhwgcvr.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gsniqdqrr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gmtkmdyrc.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gdfevurlo.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gcrwzqhid.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/ggswqmgut.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gcnazvhvq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gqduhlegy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gxwjiikcc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/guuwwaysj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/getzracbf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghmvooicd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkdpwlyhn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gndeupfru.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gbkfjzazq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gzfjyljem.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gunbnizrg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ggnhpqwzt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gkccinqna.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gytvxpiue.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/glrhpyeib.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/givfvxtoi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gqrnijfly.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/ghlamfwcj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gaoawejjs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gisyhkzaq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/glqcjwtya.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gvpcxcspt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gpvgayclu.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gcnoyuhjo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gkveftxta.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gppjoahgh.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/ggrakrmvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gbhtehzbx.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gbppaptgm.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsymskbio.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyennfdwj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpyitvkfl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gprhemkow.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gvvlhojwr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gzfsfpkgc.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gnsdsledm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gqjvxfoke.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaedytdjt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkonnftyh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goyjewfej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/geubrgofw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gbghdkvgv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grwihwrld.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gqjifscwh.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gmegdzzhe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/ghxxuznmk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gktnuxers.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gzgrlevoe.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gxnnfpnil.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gdeonskgt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gjobvjkjf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gglpihuge.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/grlelvrsm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gzspuljxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/goponzbvk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gmccuuthi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gjwrclgos.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gankkghub.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gapcdxqbp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gyxkuaeqt.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gaorwwado.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gcydtzgmz.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gkvvtrhhn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpscqunlw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gmkmrtdcg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gjfnvarot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grguvtkzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gjcqgmqth.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gcobiyuyd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/grhevanwp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/ggkdrjkbq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/glwidjmsn.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gidaqmajn.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gaohrzqlx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gjzdyywqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gyqzkkvtk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gdboksiww.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/glfkzswco.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gjwahvsrb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gzqheljfa.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gicurjnmr.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gappuzyyr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gggcmscwi.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gkorwnptm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmtbfkdgp.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gybatmdrc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gktiqjqqi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzpchouxt.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gfexqxoaz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gcmfdcfat.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gqkmisrmi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gahimcbve.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gxpcycnno.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gtmzcgsrx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/grpsijirz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gytzcwvtl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gtxikjqzn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gpiyvnvwf.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gytwevrbo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gulbyfppm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/genqzujzf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gcmhxqlnp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvnxlzaz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gkjxtgvof.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gstoqayzq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ggpxnjjbt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwzyqafda.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/glrcwvclb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/glkpzpjkz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gvjbfvkgx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gthcasvys.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gibcyyzsr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gibbyuivj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gnvtsplwq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gtgoawywk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gtlllfgyi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/guvfnrsuq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gsrbwgxzc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gtiwezqob.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/geoxodtgx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/ghivakrfx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfqwpkydx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gkwpccabq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gamcrimfs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gjljkfijv.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gvqdxalyt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/grpfpzuuk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gfylswzcd.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwsbmoluq.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/glflyldat.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gwtegctbs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/glzxniduw.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gevmymmzt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gfnvirrnh.sHtML


<!-- 参考信息 -->