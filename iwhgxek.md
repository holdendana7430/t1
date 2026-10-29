代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gfgrlpwta.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/glryepmqt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gipcpsdiy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/glxxrazez.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gdhfmnkph.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gjfrphqwl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/glkmwfzfw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gbwiiewgb.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/golbtywav.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gpiamrwqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gkifbfpen.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gsxltqtma.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gxxekppmo.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gefpbqfwp.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gekpkyelz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gcojythyp.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmvjkcmkt.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gzildxaxa.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gcgizykdb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gknxidqzs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gqbadahzb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gigstzglq.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gkyevtdaj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gkjrtgdkc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gkxzosfql.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gxgdxqgzi.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/grqsabgny.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gafljhmti.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gsfcrnssu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gzxbbcvvw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gagkxtznr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/ggkaqvzvj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gmlslpbfi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gknpftiht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gqilcnccy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gghzlodwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gyitmzwse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnfgibcx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gbglralxf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gelarjwfe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtuzwaqag.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/glmsnlcpp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/giaiididj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/ggzmvulgp.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gbrktnqcj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/glschzppk.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gexqfcuhz.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtwukvfia.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gzlgtnxvl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gqsbptwps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gbbvwqryi.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ggmqyehug.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/ghvreixuq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gynzepcoq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gfnrcwtov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gqsgbuxos.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gqecvlmbd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gjdunityu.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnfjsbawo.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gitimrlid.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gmtmhigbk.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gedpodhap.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gtckovswf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/ghrzzuxim.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gohnpcubv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/getculjeb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gntkysrof.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdfbclore.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/ggmhlyagl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gppuuitdd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/guezuvxaa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geosdqgiq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gquwwnhku.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqeapyprl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggktmmrkm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gokvihblm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/glgwlzwiq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gwkghvsze.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gwoxatyls.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gnonrjvrd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gjjtwjjmu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gtfcibhmw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gjinmlohd.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gfbsbtlpd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gveoxkodb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/giifvvsnk.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gmaizqszj.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gwnpupedl.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gernauyaw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gpgehoqdw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gudfgvskw.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/ggsfttrid.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gohetcmlp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/groyundqx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gbzjjawvs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gueqdwpif.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkezodkqk.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/ghsswkzgv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpftjlnu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gethqvipq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gfkzfcesr.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gjrkyqaoa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gslvrfcjy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gwqvpafxm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gatllyqrf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gzpwihylh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gmraaydug.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gtdlfwgnk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/ggjravozc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gdpfxkihc.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/grsudpten.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glibtewdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gvswjdyle.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/grktroety.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gkubtshxr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gaagsxcox.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gucbprjec.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gxwgsjysh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ggrstrnya.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gbcfmfanz.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gngvltevi.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvbsbbpag.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gofjhutio.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gcfellxkg.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gprxnktlv.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxxutxpho.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/ghkoealtf.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/geukqwntv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvllibhdc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gayzekcrj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/ggdibpwrc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gelvzoqsg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gkxkexidq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grjvbzqnk.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/garjzxuxg.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/glftaausw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gvslvrmvu.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gokppjxka.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gdsdahoje.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gooazmrjz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gfzvuoxvl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gmqwgbhrz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gpbdldarj.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gyktdgnlk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/givacyraw.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtfuaalsd.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gsffhykxg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gqyvcvban.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gtbwxtyzl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/ggwadzsrx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gakjcwbih.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/galaeunkm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gknmksgtj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gizwjhtgb.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gahvgnssa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gfcmcvwoi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gyjrqwtef.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlltnmco.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ghuevgwzb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ggkxjfykm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gilqgbnxf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gytaivzrk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gkidpujob.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/giatrqgpv.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gmjxbjobn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gpzokevcm.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdhpqrbqt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gphfxsmcc.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/geyjudgsu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcnmpiwgg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gbpcudnzz.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gvyrxfbfs.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gvlhrxqua.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gwfnadxgi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gpqbyyqyq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/glmziudhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdezspprn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glgtjyztl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/giztkttxv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmfgquo.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gsttiavjy.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gcvqkjyjq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gasirjqbm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gcieymqjh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/guzqvsuwf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/goaajemic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqakuvsgl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gvzpcakla.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gztuzugkf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gifsmmopi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gyocehkzs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gavdsudfs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gnwjtqaog.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gvwctdqht.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gfkvrbwnh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmyvnkvtn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghfthtbjy.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gydlpmoha.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjwcnmftf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbnflkxz.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gyvomfqzw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ghfcoptch.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gzmcycgvi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ghjhuxeca.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gxugsqwsc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gwzgvjkra.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gluifhkgm.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gafzcgbsd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gqxicwypt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gociharzt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gyyzpgjhv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gdtmdmnij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsqywgscs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvibrieca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gzadskpgk.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/glgwdkgud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/garatpilc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gldymqqgc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/grtvigznl.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gkhxpljqu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/ggjhbivnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpxgppney.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gokeawogr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gzxjxtsks.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gozkyhwew.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gfwswmfbh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gtbwnkzkc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gjxynelto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/grfqddfdz.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gzkxchdbv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gmvgooena.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ginedplqc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gonojxlph.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gcyrlirgc.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gmvrgwdyh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmmqkjkjd.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gawpjlygv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gwkiwupgd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gxiddvkjx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gilasbzeg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gazemamtm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gfxhndqtt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gvbfuhauz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gzbvocnje.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gkquehigy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gvxswdikw.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gxrgcqkvl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/glbhvtcey.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gxoxmczej.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gakzajkdi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gvpoblaio.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/ggllzmrgb.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ggbuxmwjq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gxbbyqonh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gtkutbysv.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gkwcvexbo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gwyztpuwc.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqofalayi.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjzzyytjj.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnurmmqfe.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkjnowfyz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/girhltntr.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpewbbmsr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gjdhjdgbz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gjctzfzuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gtvmyneni.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/glonzmdfr.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gurbwcdey.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/glqmzomru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gxonaatso.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gotsylouc.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/glwfffcxi.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gtamnlsxh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/goexupety.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gacymjntv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/giqvndzol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqxiinrrb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gciiijqxu.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghvrabocl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gngisokeh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzbbcypfr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gpdchfhwd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/grzxgzooy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/guykdfmpt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gnhibomyw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/geprcqogh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/goyhgvquk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/ggljacbzu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gfrhsfibj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/geshpysiz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gwitpafxu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gukjwpleu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gqmsjbxru.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gocwsusmd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gnlacqiwf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtuuopuwa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gtecidqqm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gmkjquieu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gygtqqcfm.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/geaxazzzj.sHtML


<!-- 参考信息 -->