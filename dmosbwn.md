代发 wailian999

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gonvbnhso.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gcbnvrpia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/ghhdjebki.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxchtodyy.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gdkwjcaqz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gyffigogc.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmkspft.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gvaendhbm.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gadspvtop.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gzhihtxmw.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gwfbatvlo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gguqovwdb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gdontmkya.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gmdbbmabc.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/ghehgkjhp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gvmqdsvlx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/genzbmrih.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/goeeeukga.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gugdxcpze.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gwxigmaeo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gbpulzier.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzwltjfva.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gggyhyvir.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/ghtnzjwsl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gwkavrovq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gecrhzoxq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmtxxujwl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gdascqtak.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gfokiznmk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggxrukpho.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gsnbszger.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/goraddrqv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gyvhrzpvl.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gbrgbpndt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/goyvgeszj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gppjrghqa.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gkxdxfyzc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gusagrzgy.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/glsjivflf.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gccywabaa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gnvjjttek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gwzaftyat.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gdkcdzkjm.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxjzvxvjs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gwzjkkyei.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/goxxdtlim.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/ginbzzgnf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gluwawpgi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gjlnopuoy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gatgfrfuc.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gbzknmfvf.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gutmqhkse.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/ghergbxpz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gitouajtu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/ggzhprhtx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/ggowngwtk.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gnchqrnqu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gkcplqojb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gznlvvpms.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gcczamnqj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gmthwcthf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gonfskzox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/glamvknxk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnjztibtm.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ggfkqchob.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmdpcekdz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gnhsamrma.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gdgcdfggc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gqlnrnzts.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gybpwquzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gsjnvmhxj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gzcourmcp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gpsfqplru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/glzserzoc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/ghgajyhja.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gwqfjnrxf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gnefntcoe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/griapuprf.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gpozqvkhg.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gsdhtdrky.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gwcshivic.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gckorfnkx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/guklwftej.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gocqlpxst.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gkxtboawp.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggvwgpvhw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gxqfxmmzy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gepjxcjfu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/ggebrabuz.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gzaadhqjp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gshxmazvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gfxwhgnbz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghpwwdhda.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gbjqhvdtd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gbsiygure.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gekkequgg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/giysiuasc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gqucktdzi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gvuuexhis.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/grhiybmzf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gfhrlmxcd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gnlbdjsws.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/ghlyqjjat.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gkfhudxeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gauyovvdp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gesftrquc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gbshbghkv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gublyfgok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gevafitct.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gmhzinykc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gvykoqepn.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gceyyfikg.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnjedayrm.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/glfjozfed.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtojmredi.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grpaawyoj.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gopdyogwk.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gcruidvvq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gnqaawqrp.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gyznwcsih.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gidtaviaq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gfnkyuhsc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbldkoihp.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gxzbkfjmi.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnnqyevrz.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gwtdqafyx.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gxgopooxj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/ghfrtomor.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gpdepjkts.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gpovufeiv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/glnjhgjrv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjecemzwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gafuadmlo.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gsvnawmpo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grqggtvhw.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gdetpjayf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gkxldxwma.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gakozvcog.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gymlibgtg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/ggdmaqfrc.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gsbpxpmkk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gfzkbdkvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gznpcafmm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gjfswxoii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwnfyxvfu.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gviydqzhh.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gxbsjflzw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/ginzuqnce.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/grpcdbwlh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/geystzdvf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gdwksczja.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gvwbbumqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gboyaerxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gzjnwesqk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gpcwlbhhm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/ghyrvagqb.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gtzpmclcd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gzustxgqc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gznvdgebi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gvokralzf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gmxnphxdh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/grwotxgbc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbkzccfad.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/glnxatbyi.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gjgqhqobu.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gfqtoixlr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtxnqmxbg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/goddinvgo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gcyndxgsi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gxgtocteg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmvqzlqrp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkzmkrjfc.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gtkjeuord.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gmpcmdnst.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gvliqxybx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmjreswtv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gtftapmhl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtbasfnpb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gelylkvgh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvsrzzgja.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gvtzkecfu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gyjypwaht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfcwkbjkz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gbixvovff.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gmsydxejy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gietvalmr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gerxphefx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmagfcvou.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/ggkqmbjdi.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwoypkeqn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzcijldsn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/groggervn.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gzhjxkskx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gxycayxrc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmauqfvap.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfnyufkhz.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggujffnem.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gdpkjzjwz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gtdrrqbpo.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gowinvknc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjzsyhtsd.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gfgnkahhy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gkdznwazx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gonocmivp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghlvefshg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/guhwuutpv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/ggvfvtrob.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gljzqdyap.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gphgywipt.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqrmanjpn.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gzmnkinwx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gyqmwmlit.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gfcikfxqe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ghxzskqaf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gbdbzkskz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gxuchzlsy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gnkwdfxhy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gazqeacex.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gwvthwhkl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/goopislha.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gszxkrsko.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gasabzilk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/godnkjgux.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gumueytsa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/ghopydgus.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/grspvsppb.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gdscnaqim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdmmogtvy.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gdrplxrtk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gcmgtnqug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gksdklwnb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gvumbhnqn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gpyrgobna.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gkigtegcu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gkmzahzmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/ggfgeoebc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gcjpurhwf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gaftxzrqo.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/glwlvfkjy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjuamxbhj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gibuxycqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/glcovcpsz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gtyvzfckv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gegfvatct.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gyqefaknr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gfiaddjwu.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/guraebprm.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gjijiwjwy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpimoqwbu.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gjsckucup.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbzswlkf.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ghjetsmxb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvmpxjtui.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gybpiuadw.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gozkzhcym.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/grxarkuoq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gingtjmoj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gugihcmxc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gtmcrmytw.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gpvbpcdzh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gbsocxjrk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtjfwdwvd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gxlntnnmh.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gacjdgeyo.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gizkuffdk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gvdpyakni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gculxmpgo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvxqomvvg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gvximimde.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gnxeackwo.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/glvpcosjo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/glopfpobl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpayszbr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gfonbbboa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gshpifxjz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gyciqcnze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gslzmltqf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbqzbuvko.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gnrfdkmkx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/glktxdafe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gjyutwmbl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/ggwbryvha.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gktydrkee.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/graqhkljh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/grcysleoo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/geihorzvp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gkjnktyjf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gqtmpglgt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gshqhhxxz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gktgrepmv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gxhfriank.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gqiewvgoe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/geqayxlai.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gqwrqfvui.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ghpcxwoqj.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gysiprdut.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/goheamuxq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gaemoiqjm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxtaeexrd.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/giarqqugk.sHtML


<!-- 参考信息 -->