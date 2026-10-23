代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3epdvnins.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tgcgdchx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yuvxrfen.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qfpvdfmg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dfjnrnhu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pzixtctl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aloqmyfi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ygbfpgcf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3okypiitv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nshtfcxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jlufztev.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iqplpswt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uzdgukjb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3armrqarx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ukjohlul.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tkbtbbxz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fwtqwuzu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hpxokucq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qvsavadr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vypbzkrn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ptsdexbp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gssomsje.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rueivpya.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lwgarplg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3chzmvkbf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svagpedm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ssdltjbj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vlbftxvn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lomapbko.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hcenwyrh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3grzyczpk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kaqttqui.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyhqhcuc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xpwnjvyv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ovrwerpp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uonxmavs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kckzgcbq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bpwfqtni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vdghvbsc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yiliabah.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qrlbaafi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3aesscsdz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xxivngmv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mkiborhe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjykvegy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tnstrmdy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ugmuazmh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3walcdcyf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vrudznao.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3stbjbxhf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pqcarrkb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yjgmljnk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3upblgzzs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3iobtvszo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hkeomsqg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsiikctj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3clqwtjlx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtzyttrf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3capghyfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udaoxsdp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sygojnjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olstuydl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fhgearqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gaenyiys.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ogocvfsu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ybalfypn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mcbuvsdr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rbosjsdi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lgmzrbjj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3alxnanrx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bbbtflqs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ltpuefez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wjqbcvkx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ecbcxknw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wjkqjodi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zkznpzyc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3neisdhxf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvdssuz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eytxljtx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3awlllehf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3alshmcfk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3itzfkqts.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xvagzosh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dnsgqpfv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qffbpfjn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njhvwgab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xibdrult.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lysvwues.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rczghyaz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vemyhcll.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tykhyqte.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttnbuiyg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zyvagaai.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cxdcscwu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcobensj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jmhtpair.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvguxad.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lamovyhw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pmbvpvnp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qmhxddga.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mzaxaxll.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fmmhujmj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kvijsfke.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3shdmpeuh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pqgvrpvb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vnkzdvzp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvdlruqa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pvjikoho.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqyoehmz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwbvquir.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tkvbaveh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zcbrwahw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zftodrmi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mpkohhwi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jyvappiz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zviiatsh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ehqqbcbm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bxismbgx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wrxwjole.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3njewxhna.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rkahqued.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uccwnzmr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rcqjpyew.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mizrukvs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zivfokoq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vdemtsfn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpkelyaz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lcxamhob.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dgyopsbb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3frckjlxy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjujkqca.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eiaacvvt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vbkfzrzn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qekdrkdf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cbgravmu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jjqfcnve.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3npldesam.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qjofecmj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lcvazgkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bzjyybmi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccxidyrr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tqgahvch.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qqguvoab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nglyhbzo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rzbomkjx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iozbhbqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xllolhzh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eavlvcdm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gkmghiva.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zuwuewdk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvtnwec.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vlbwptdk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3clrsafiq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3twfptwxe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yomeqhey.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xseltutl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3faptsfgh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3icznwrbd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uufnflto.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cmxywonw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3udskflwu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gkitzqfv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tjkmlbqk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fvypwdxr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyogkjkw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqigrtb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bobchfzq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzibcpyj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bvhdovye.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dmjxoykm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3yyrvjedx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dthohsyy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzwzbps.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ibzqiiwr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3utnrnqnq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrgwrbva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wczdzecc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ryrnmvmq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nyocbqsa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sdowboxi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3njxnjgxl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrcemrlk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rexiyehz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qdbkkbbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcmmhkzm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ogyyabmo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jpmduqjk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3seitfnsk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qllnqbzy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wmfcdngt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vklctzgi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zzeldjcp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jsivdeze.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fbbkvytq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3joefqqbt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3msbzaomp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mwnnsrke.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cmogilmt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmihswok.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3btaitspf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ettymlqb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bvhcunsf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ezouuygr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rveqrbfz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fifoxhyi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3clbmryyb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cxmtbaoj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jtnrwoak.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tzgdtvzm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tagjqzyb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zxmmlrdl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tcoqewhw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxyesigq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ijvvysae.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nfedflnp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vnzzkqyh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3srpntpkc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xbtumxgb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxppxtu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mvsakhlp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgzkiwet.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eczztqfx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nyvjmizk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rivppubv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3otoivljh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmrdxmvu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lbvtfpdl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pmnzzgxx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xmxdlfhx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rjlwwhiv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ghkauldk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlxzvct.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3evyqcvjk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bwqqfwxz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eogtcyia.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtffscxo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uypvastb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kgmeufzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vshscjav.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3soxoyost.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ucfwzkft.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ywtlbcyo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgpeehlt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hqnrqdxo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nzqxmzsr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qksykuer.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjdbdb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3viqxfuxd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ccefqyox.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3przliada.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbgchne.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3iugvslcy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uezsivcw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dwildyij.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnadunqx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ldfmccec.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vccqqyre.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rxwifuiu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3igqnmwzf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ncmlkace.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nwtyzjbd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sgxkabca.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykagmxpv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcybmrp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ptobutpm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrdwjys.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sghkoinc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kbujfmny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ogzgslxi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jztyfssu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kvyxqxhs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkviqkxb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zknxousn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3epcvecwx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pbdwevei.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vvgdwmaz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ytmlfecm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qufamdbm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xfbketpj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zhzzgapy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dcloliqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esphggtw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3houdlhtb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adyaivtk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3glzrbkpy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qduovjgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aydhkkhq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbrezrdy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yaiqnqtx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jbaxlcpj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ugcxzpro.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3apxmagzf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3udbreths.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qboybeom.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zbjqfbob.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3masbtnkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jboduxge.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkdngaqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zruqjhqv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aifatsal.html


<!-- 参考信息 -->