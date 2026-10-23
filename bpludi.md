代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmdsafxp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xjxragvk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3morczhcv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3syamaymf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fwzlwjbh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cpwlplmc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fffzddpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jucyhatg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ltqkrhbp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3htqptzhl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zbckaroz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dmdjdelm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cwpbzyfc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mwblzlcb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fezexavt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jrwdqaib.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mkivitol.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uybqyeio.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wcikgbwx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3anmrwwdq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3somjnaok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvdtndyc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mxyeicuo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nebxdfnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkmykpps.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3obcmvfny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kluophkp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dlaosihr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wolyyecb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3eosmbcew.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3inljquao.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3upebcwdx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ndhhfoby.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wqlszmve.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3waokszgj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bezlhhlt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lmztagxm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jszrlsbr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vnpwwwpx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ffzvxxtz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kfxsmuwl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dzljtciz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bfaagxzi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fcmyanoo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gocyrezv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rxlzizlx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3blysqmmq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mepbhfhf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3milqfltn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kmwcdawo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3blywtard.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fwshjwgh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kmhkcgke.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jsujdhjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gsqlwsqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3revildvm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jpvctica.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3livnknyt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3odrlgywy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yyduqibd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cpcwntzi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yynkkyrg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oleoiwvh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mkmfqqkf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3guqgtfvx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yaikbquy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3rikqgfhs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xohyybnq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qvjsicsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3almjiyqo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhwprjck.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anzubmvg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qaxxcdpx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jdknibag.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eiizushc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kbdidgqb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ppchfkrf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlnbbqh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3aecmmtik.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bclefyie.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yxysimsa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dovgsgyh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aaozxshj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwbdnbgx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bhjhxudx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qfgaljdx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xevqyuiy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcurhfjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3goidnfdz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kkqfuyfa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3byqavvsx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3oaykhmzt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jvktgrqs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3aqnrakef.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dtakljgc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qzbizxvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kvscpedq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qvjuihhs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3plhmipcq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nvurnwyx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wsydtpts.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jxmgbyzj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wpdghipi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqlmxwke.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbiybjh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pydodupu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dltcrhju.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vseeuipu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3nrqniwbl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vetkrhfq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qihsjxqn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hvhwtoec.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tzckmssb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jnqxdrzs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jzvletsl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3edofznuq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hnjuunpu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmjumlkg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3quvlfupd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wvddwoxa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ggqlotjl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zxjfnjhf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wzqeyquv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vkljxkus.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3szwiwilu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wgjtjfan.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jsaejrfn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vueqnkwd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3orlsqmuk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rmfxmezd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mmxusvfr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wtiwyxis.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sngflctf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ifglibxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pbedonsn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nrkxwsrh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bazsrpdv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vxqsqaey.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vifhqlar.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hwjxahmr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qlnfglwy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wvjltyhx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qmuljpng.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kahhbgaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jvwitddx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jwekeqar.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cjmmlbrz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mhycsalq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qwuldnag.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3senpikty.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydniczgx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3egflbzyi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3toydsqfp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vyjxntcf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxgupyvt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mbjdjxdi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zhgvitgk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pxnlzykv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fsqvijmo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sepirqgz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpvzehig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuczjpjf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bacdyzpv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zcqpxoil.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjtilvi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nvcesogp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mkagjrih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pumrnkst.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jdhpqmsg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvezdx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bzejtvpw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ojalsymo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wftrtqni.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sphifkdm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txdslyim.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aatyiljl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yydmbdsu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ematltpx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qdynswtd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jiheyujp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3teietmcl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3npiaafrn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpqhakn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovtnteot.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qjphxyke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3waizhikk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xgicymuw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hbozjpil.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3trdekxzv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pitjkoyz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3aiqshkix.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvftrt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmsivlf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3osgdcxad.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifoxvkmb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqbizmsh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3atuyiwvy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3frsbbbbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3tqfblecs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3horvkxpq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kjliyybv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dzxoddfv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qdvxeudz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lftrlkbc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvwjyyi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yzzymyyq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hgiigvsh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mohyoiwm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3anrkfohw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kpjammqa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rkyooftl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3azzplwug.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3aekermgw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3boubaeow.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nikqrqwg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dxtlvuyt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgedgpex.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gpnaabnc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bgivjhld.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uousfxtr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wwychkki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3okaljomx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mqhwsqng.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tgdzbtun.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ajjnuuro.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gpavkzex.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uvziqgoa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mgygtznx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3voiyohed.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3giiztkpb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxkxxje.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvwezlxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yflqjpch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3besgvttv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mraisfal.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rnocngkx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bzgybwci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dtuoepjt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ryldoaiq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hcbaudth.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3iobigbzh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlnjsykq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxersymo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ulamenis.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ruliydno.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zjvqqfsr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxsoyso.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xnulvuid.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yiknicrw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3heebcjsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgehjkbs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tobpwosc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wxtqinuc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wgdyjbte.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rdtcixup.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uvsfljkc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bjxysvhg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjzeoog.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cnpfeefa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtdinbh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3krhyfcpr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3eccalmfz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxtysrvn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dcxhtiws.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtdzgbml.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ovkoqowf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jwqgdaxu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdzgzljo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gkiurpdg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gsyjvfsx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yodtcged.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3adxsuhku.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uejpfraq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3junrzkuw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qdyeiyuu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xdwpmuhp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vptmvgpq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qejzzgai.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jyqkyiof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyzczpv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pmagydpn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tnmsnguq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcchpqda.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqrdrgbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjsstigu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3raargmfs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jjuzcolx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ktnczkjy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yyoqbwek.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbtqepi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3znwmlxzt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mwchqdmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgreetoa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3deqsfcss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqkrdwtf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tzkcxptl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rhjllein.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wytksizk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ranpvhpg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nedgpiio.html


<!-- 参考信息 -->