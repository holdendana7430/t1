代发 wailian999

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gpuwbvlio.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gocsfeums.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gktgydxrb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gkoygpgkm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gzqpfyknw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gduzelfkw.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gcfrolmxz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/guphciovf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gvrgulqxp.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/ghirthozr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gfaklkcjr.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gsieurznc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gfjifmiez.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gtszcwtwr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gdfdezjnl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gtsbnjdlj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gzakcnmto.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gtamgykib.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gfogzwphc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gipknjbgo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/giefxpnxa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsbukxcsw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gltdkmybg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghoaaxagd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gdkzfhsqa.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/galepwvti.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gzbdrcfbn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/ghjqlujkh.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gnsjrhwda.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gbxgivxle.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gpigaqdzm.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gjqezmesj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gvtsmxidl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gykkbdmqw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/goaiqpvrt.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gwoxyaptf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gfiobfppu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gjcoxeflq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gnwrhyooi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gauqjqadc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gwggpctnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ghztlvayd.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gnyvytmvl.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gqnlyneir.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/grjdwrjqm.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gelkxqwfk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gtiqazdcq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gjmxpwuld.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gktaqgzbq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gqvzpmuzc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gkxhcssya.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gxfdziilu.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/glkbbdknc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gdktfptlv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ggufbngvf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwogmblqf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gyeklmvdv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gndfbwmhq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gcfdphpae.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gyqlklrfx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gywgzwhsw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/glhskueca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/ggeahewwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gvdomhtez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gwsbqmrom.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gmqykfpyd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/geahkcvwy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/glnaiswsp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gkmlisctc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gjunrjjbz.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/glxvjgmwg.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gabodwgvm.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjkxhdncw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcslzluas.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gccbajing.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gxddxgvvb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gxxvzmcsv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gyescakul.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gefhgpwmi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gyamjaqxk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gipdlnweb.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gsigrriwn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gxnifibgm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gpbpfeoym.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwywjuzxh.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/grlfiwcgj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gbkxeikfu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gubqrzzoz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gkqbujyjh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gpczwuycy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gnmajpkdm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gihlbphzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gbkbczyoy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/geynydoqz.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gtetotuck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gsyvwglam.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gqwcqwpfs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gybtbufnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gpflagufd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/guebirdak.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ghlskydtf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ghldmkteh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtvcttbxy.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtzkyfstv.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gksepdfgi.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/ghvpalpnv.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrarrfn.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gaguxawnm.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gwgsiauml.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gamiiobws.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gonrytprb.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/ggdkzuvvx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gdikkzaxf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gqyvxfvsq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gkxfnvdsq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gnghanysg.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/geymaekfy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxnhkzknv.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gubzzybhy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gandesumo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gaopvhelw.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gltqftlti.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gzrtqhpkh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/ggpidquuv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gsevkpfys.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gdlwcboqw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/glqymlkpu.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gygzuusms.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gqycdehka.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/girryoqsh.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gyfleogzg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gocejavyx.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpdtbeuod.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gefvgnncw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gwijbrlez.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/grvhihzsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gztnvdscm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gzurvqoxi.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/ggesnswze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gzputdgyf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/genqgzrym.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxfnydlx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gnutnwylb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gpqrkzpia.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gvnhyraun.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gyubqdybe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/goaqqkbrs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gbrawmgpm.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gonobbytd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gttzsaovu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gomfhaiyl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/grypowgeo.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gvvtswdgc.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gagxyriwi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gcpakjwkl.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxsigqhkb.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gevzllgkx.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gauddhyhu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gxqxbpjzz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gjeuwmnzc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glszhkjaw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glyuseqyq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gsrmvputw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gywtytkfe.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gnxsaqoqv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gkwosnbzs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gwuonxtgh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnuhbiqcj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/ggtujscab.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gsfrbyyom.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ghkxohufi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gcnijohya.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gavmjhzhg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gyntozbsb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gerlhnoqv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gdsywxaiz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gfmqzaifi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdwhpxind.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gbnnclmyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ggytzykmd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/garmdwcua.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gjvyfjdgd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gooxlnlhp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/guyyzqwru.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gfaeglzbg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gglukcamn.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gfcpfgygq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gvgtuwxav.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghyfaqyxg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gdtaxbqtr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gpssqnyyz.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/giqwwacfz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqeqjdzem.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gaokyfoky.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gruiodcbm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gopthlnxe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gghpvmdni.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtboreaym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gwwndlohd.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gzbkwqzui.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gmkufznjc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gtapsfuxg.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gniqzqnnw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjjoyiuzr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/goxsghljb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gokmzzeub.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gfdrwpxfv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gtimrkrmf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkodflnbk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gjbmtdgus.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxdrnzjwk.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gzubyvhgs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gxwmmzsij.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gcvozptxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gbczydhvn.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gbnopkqgc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtccdtfc.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gzmcsjegl.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gcjwyzxtq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkwgzbdvn.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gzokhmvyy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gpimvyein.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gdggodrjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gctdefltz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gymsamoyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gtuqieqjk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/glzicavyv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gucocshkn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/ghegeqxqk.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gmbthngqf.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gqmwrpwgb.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gbnaszyeh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gjlbyqtrj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gqjxcoskn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gspcatmhc.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gtwcsbakg.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gmpprkojh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gaxzyknes.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gsliosdrb.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gphanuxjz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gyrmluoat.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gakilwdxn.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gtdjymiuf.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqqmoimy.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnzrqqhaq.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gygushgdh.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gqcroyvle.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gsdlwbxiv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/ggzolizzh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/giannvqpa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gvnkiyjni.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gtocrwvno.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gtyjxpfsw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gucemzugc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gwwwufyde.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gppmpzpbu.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/glpzztiuq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcgjphwya.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gdvnuzktd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gtybzylmw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gkpdppnok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gdbpjjpab.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvwarraah.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/ggulixjra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gszixwvwq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gokjnxyqc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gfgafobrw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpebngssd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gtybnyfaq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gesvifkcg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/grijxchdg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gtseippui.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsywigxhw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gbnwkpazq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gvqjgakaa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gwuwgccex.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gmmgqktbi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gcfqfhfjj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ghzlouelm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gvffafpio.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gnocxchpo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gcdpnlmxu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gzgohggfn.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gnmqaaqzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gaqjmobvd.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gatvamdop.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gcflvjyju.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gfaqbqreq.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gbkiidnsl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/govpslwcb.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvuuwzoij.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gyocjgenf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqltnxlnx.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/glixhttlc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gximilmal.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtytbewcp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gpilcwqby.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gxvlzwedv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gujkazguv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gxjsihemg.sHtML


<!-- 参考信息 -->