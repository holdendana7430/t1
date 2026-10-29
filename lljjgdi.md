代发 wailian999

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gebfsmmcv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/goslnzmtq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gfumrqacz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gcaasqvbh.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gqnefcyiv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gynlhzlxk.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/goufjrdaz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gvbltiecz.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbqnyhobg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gbmyedxwa.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gpqbezwpd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gzelpjtjv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gqyuggjze.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/ghwmxewel.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gnebsuvna.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/grduvttik.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gejajgszg.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gibwhfinr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gdiyhxpjy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/grqvynkzq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gtjcnfrdd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gfozvugsp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/guwjztzhk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gbswbkikz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gvpqcqyny.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gqklblhna.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcsctqsnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gulcsfaay.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gdlhyqaqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gktupyrkb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtaraopyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzgybqqts.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtnsehnfi.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gpkxvzfpv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gipvexybs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gnxacqwty.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/guztoypmh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/ganxmtuvf.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gxgeenymx.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gdyzuonhx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gbwnbggnt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gwlsevvbh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gwrvmfonk.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gdfqyitts.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gxpkanpqd.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gkfwleycd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gtaioedab.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gyedrzqbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gyhwbgkvq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gpcijiffc.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gehqxpwmg.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/glfmmowgf.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gpwkyuzzx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gpkpkymfr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gcpsveyzi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gztdphlyl.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/glwpemozm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/galptkpfx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/goosehxdn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gccmqqzuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gbekmdjuu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gsvycnnrd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gosbcwdbd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grdcwplpp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gulcyzbsj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmgwioxcu.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gpjzlpnrk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gmvtgxovs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gqgzjpgoc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gashrjjxd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gkkagsdjl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/ghxgupvak.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/glnzktgqo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gsqxxwfxw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gnxholjdr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gydfokwhr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gojpkmxvg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gqfpeijbz.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gtugukjpj.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gzuqyrftj.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gcxoaeduo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/ggauryysy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/glctaxzds.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gufmeovhs.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gvmeqijit.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsgxvnjtj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gqpqgjqea.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gvzoklxjd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gajrdelfo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gztjfdibo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gjbonalrq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/giztpprml.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gksqicwax.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/grbqzwusb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvwrwpuuu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gekcwignx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gbtzjwqbi.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/grpnirdyj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gnsnvhhdm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/glxtyjzyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/ggmgjpssu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gslurrhds.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gfgkplsfe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gomkyfktp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gpbckeldt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdfphjvmh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gsohlddhr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/ggnmwfdcc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gowfjlbps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtizyuzgw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gzkyxfrua.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtbscpp.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvufiqupl.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjuiwybst.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gveylosfw.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/genzuawja.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gmhjgdpqr.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gkvbbccrc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gfmpozbxj.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gqplbtseg.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gkmrvbnrz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gzrdtsazj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gpctcxlnu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdpxwcufp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnkyzqxww.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gvxfoqujf.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gwcrrxjeq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gydxpxosv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/glgizikrs.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ghfawrocj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/genifmnyf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/ghgthsmqb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/guxlyytxp.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfqjcll.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gojruydja.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gtizgldal.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gjqxnjmpa.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gjptfntmm.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gnfgjfded.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmdnarizj.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gurbnvigw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gzbzwcttu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gwtpjwkpg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/ggsiycbbv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/giudciqcd.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gzwgockjb.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/guaefjbqs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/ghaabqsmd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/glkxzhfmb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gbmctgsrx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/getteorup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggrspeqww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gjekccvbx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/garnimpsl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gbrzcnnlz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gflqbpahz.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gljwmpsdx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/glccfdwir.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gnxrwxusd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gdwwplmxk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gmtabuhge.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/ggtjpmjxi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/ghgknlory.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gidyvxqsn.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gtxvjzwxe.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwkhrxkgx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gaatejskv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gteaqjlcj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpjkkikqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gougedwai.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gsvahljtr.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/godouesvp.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/govsejmyv.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/goqikzmya.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gonnqwkri.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gcbembzkq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gebxuvxrq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqwqwngpi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gvsegyyfk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gecnadxyg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gayxrgjrf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmlpzuf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gonexbkyn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gedknawmk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gufnyhjmg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxbpmqlwk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gkqqudoyf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/goewunrll.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghrlosijl.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gxjypxuoi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guehxctaa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gokaebfst.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvccpmwsb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gavuiazty.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/glxorgbsl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmyaddptt.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gibzzvyjw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gkrjipzba.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gzolkkkrr.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gcppqshrf.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gdzerlzqm.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gxxrqulcj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gmwqmjsyd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/giyirtikb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gsngiapnk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gibmyhboq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/guroiawkp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gbwqbqqks.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gxrmhngnd.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/guzmrzduh.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gefilgzgt.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gaxgscbyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gnqmjcqcm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvymzrrc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gnyozeoqk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gxdmdxrhu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcyzlsvkl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gdjvcjuhd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gxfiaibxt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gkyadbeva.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gwmhfiqzc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/grzpdzmbz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gfgkdgwci.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gsvplzoyx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjymclrdq.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gvcwnejmx.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gmvjcigtl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/glntrirvo.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gcxfptpjk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gisvlsqsl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gvatyekhs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gpjyncmwb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gncftvzrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gvnyzlwgb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gbdnkujwn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gdcwctwiq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gqxyfjami.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gkddmwenr.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxonuoebi.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/ggylprjrq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gnngiblyw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gztanbsde.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gxxcpceyl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/ggkkvjdgd.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gfjfcstqw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gauwwfdbj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gwedhnktq.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/grsxfouwy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxxnhubro.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/guqgnazai.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghrftnteu.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gwlpyakru.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfzmpzwnt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gxdwwnxru.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gaouumxni.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/grvtapddy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gytzofaft.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/ghefmagpi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gyfpjfzhv.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gxwabdzwf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gwylfiqia.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gdqofildx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ggjrpukga.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gjakeayzv.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gzfkxmxng.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gpjsnlczs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnuiwflk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gmnwdpgbl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ggsqmvbes.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gmwhwvrms.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gfwmprwvw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gqldixyjb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gntkmqcfq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gztnugmrr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/ggmerduok.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghoghlrjk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxankexfs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvatgnlug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/glohhfmhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gzdojspwa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gdtenpsga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/ggchhoicm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/goythtvjy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gsjjrmbyn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gjctzpbsm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/ggzlqeibp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gxppmlyiv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzkzptgsy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gspewfczq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/giqaahudz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gqompuuyc.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gzyiazhit.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gbwsqbziz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gndrhrjkc.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbqyazjtw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxywapju.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/giketmcvn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gzvrtrblj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gfkgtvssa.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gpycjcpkm.sHtML


<!-- 参考信息 -->