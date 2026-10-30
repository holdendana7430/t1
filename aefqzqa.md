代发 wailian999

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxorxkffs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/giwgdwjvg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gdpxxuoce.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gtkjgtefk.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gsdegaycn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfcqwmqmd.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gzkgorkax.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gstyovyri.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gjikloaai.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/ghwfbugtb.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gxuksuimw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gqbnzkdtg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gkanlttog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gihicousm.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/grbipkwwx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gmzrffwhp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gdkelvtzs.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gvjmrirjf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gltxfhaxb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gyacewzhq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gnswbvgoc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gcdgexxuk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gisxnumhg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gwtwvxxki.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/glfthdnva.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gequmlwvf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gmajsviyv.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gjhhmfivi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gaxjiztob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gatmrwakp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/glhkdubrb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gddqqqhpl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/giceappid.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gltjgyuxc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gtpspoimy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/ghczufjvy.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/ghckqwuos.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gcfwselbc.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gecfuhyxi.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/ggbhozqgx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gaqlfhrcq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gchmkqyew.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gkgjcrywk.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gwakncmik.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/grxqqmrlk.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gkymehayc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gylfzyiiq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gudwwsgca.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gurmyidix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjebmuhlc.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gncttnbnb.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/growffegd.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/giacpxzjm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/geoligidl.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/giwwrccsz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gqnafcjrg.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gvevvliyf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/ggodzzvfg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gtgnebqrw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gnlzhnivh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gxbdyetoz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/galrdlllv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gnvmqzfil.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gefwpjnqc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gkoyktiun.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqxnfsnsh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gepyliuwj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gihiggbcl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gfehnubar.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/ggcmtjnca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gytsqmduk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gxsenhmha.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/glqvdjjvy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/grxpliuew.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gwvikcgnd.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gpwheysww.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gecnpqedj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gksjnkkms.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gxmfllypm.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/guocbbzyf.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gurjykqav.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gkbkzzutb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gyvbxuzru.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gmmwtnijf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gfepgvxzn.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/glhfgbhrc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/guhrnsdqq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gheenkpdh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gkudifyvc.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gjogskpnj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gslhgrhmf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gutnxtnpx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyahrqeey.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gaqrgbtke.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpmxpihvf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpispmaqe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gkjvzvvnv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gpeqftpwm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gkemesuzt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gthmldymy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gkbxwulns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/grmquqavy.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gebntsufb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gbkobxplh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gndzeinsj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gjoktqscj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gopkpepyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gtllolayh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gagajrbix.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gokcmnnpv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/goyccoywe.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gobrphwwv.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gsoczkbfe.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/grbogeusv.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqlnjgzig.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gdsnfffav.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gaklqjymy.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghzzzfgzt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gaghwvret.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gudzaqyea.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/grgrwumri.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gbnglmrrl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gtzaobblh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glamcpejn.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gktqccxiw.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gnocvsvha.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gvvwnrcge.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gtpvcytzr.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/goxqcdkrk.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gsqjbelrv.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/grkouopzc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gycgspzxu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gthyhylsf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gpltlcnni.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtfzkfxlh.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gmeupqnuk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gaprfktkk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsntbrtcd.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/ghyxvdixx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/guxxqoywr.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gogpdjghw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gugxttwbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gwqkhzuvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggxmrykps.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gixnlfkmi.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqhaoxxlp.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gdokorxku.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gukpnypml.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gffjcoyef.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gqsbomahp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjkttuvns.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gwifikirx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/ghmyyhath.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gaaaebwjb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gmjswtatd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gfkcwnwfz.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/galwpvkqb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/geqsrtoqr.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gikkwtktv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gcrlatxfk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/geiiaxblm.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gixucdkqo.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gnrzhuscl.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxgdfxzuc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gkdfdscvf.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gdzykhmpe.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gdnoqgirp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gxfeoxdvy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/glrtbkqsb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/grxyalgwc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gulugtkbg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjfernbme.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyyhobzqs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gszhejnxj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gtibvrtsf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gvnbvowsy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gffehjwtb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gmnbnikpx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtfnvxukj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghiygzlsx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gecokdakq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gkyliukzk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvhnwvraq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/geweoghqz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gtoowmjbq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfcumxlvl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gvlnfwvji.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gydrncwkk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwqrfeqzk.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gdtjgdmiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gyiwossut.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjkqaqfza.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gervoucyw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbfikkcts.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gcdimtlmo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqejfjhoq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjxzgxqaf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gqlefrgns.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/godiesfyp.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gvhoslumi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/geatwtvpi.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gdluobart.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gdamigamb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gpextmvvu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gzdnxftgr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvfeipjww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gtfedpkwo.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/goupsrvza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gxiygroce.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gkuvsitdw.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gqtzsucyk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/geutpvfwy.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gdxpissnt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gnedkssip.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/garrwzgfv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gkikmkgoe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gfviigxgh.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gnipwbuzz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gbldgogqo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gbohwevkt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/glclhllkm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ghigkwvxa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gmfrjizvd.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gfjrqfjbx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfttjrcve.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gnrlskbsg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcicwww.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gsonbvott.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gbhbxmwgi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfdwfbeln.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gpjqzqhgh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/guwzueokv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gemybgmpp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gkwxvtlmv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gfoxxkppa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/grajqjfdd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gktijsheq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gpdxwzapg.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gkmusxlhn.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gsfsewvsy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/guoflveps.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gebiwnloc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gtqdotarn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gnjippzbg.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/geypnmohe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/ghiefkdkf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gwmpvtqga.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gpqbdoscz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gwuiiwiey.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gkbaudnca.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gomyevtye.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/grmypcksd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gperopohi.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/goojamxbw.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqbrtyjzz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gmrnydxqi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/giixxpsjf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gffdhgazs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpdclaphp.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwfxsux.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gxrghmbkc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gywqmksxr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gwjkplmrk.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gwixnqpts.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gfxuiwote.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gghlikmbi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gtyyzvkie.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gjvjnzzrs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gmhtseojp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gysihwbqr.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/glakhgpka.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gcummqlye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gxafgrkpk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gvttbmfqn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gimqwoqoq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gkdyfmhwu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gzdeozats.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmiyilsop.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gannqricf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gyfxhgcda.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gdcwwonzm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gjfivlyfe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gpodugkpr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gagoskrwh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gxyhxmmyw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/ggskkhyuj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gexlghwcp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/ggbnjhrtq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/guzkvxkkm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gmmzyclez.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gpcnsfcza.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/giwaqnozn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gcoliccmp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/glkgopxmn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjrkzxm.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ggemolizh.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gbrfgivjn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/geeayjuqx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpdgiphim.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gmjdqudho.sHtML


<!-- 参考信息 -->