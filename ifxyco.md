代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lqorlodn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vqgkxvrn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wgzwzaxp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hnhonwzs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kqwmbzth.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2viazxtgx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2stssnzpe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mbgbobtg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jljfefws.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2chgjimug.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bwooaobn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jejuyivt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2myrjbchc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dkdacnjd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fpsfhpvb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rtomdnns.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2irobufck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wvrngfnv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gmewbjbi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xeluhdvk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khawaqwy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cyvtkxgl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bhqlgpjw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vdhztila.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nroylwgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uigrbzqq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kcxmsxdb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jlsegghe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xkqgtoue.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nyripydq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cttiilbr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nhxsgunm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fdexfiif.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tjoeemay.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xxggaemr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bvxbmrmn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ldmqvggh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlsbyzox.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2siohviuu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pphxnoqi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wtylnrhe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lvoanitp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xkzdmeue.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nxvedpog.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fqicyegv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cpfyucos.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mzmwxmbi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nvycjadp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2exbpwpat.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2memlzjfc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vkofagbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrjtseye.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yylfqyjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wobjfsbp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uyncpmvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2inhjlkja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pmwujbjw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jlosentq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2svmwllbe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2avvnitfp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2insspsxh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mdzaylyr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pqgkukfq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2afmhtoqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2drqsslrt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zgyxzbnb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lfbrhjpo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zkushvoo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bujlrjlr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxdwujb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2olhyrrky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2iovrgsli.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uklcdrdk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmejamkg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2huvukupr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zrmzddsq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2azpyxyvz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ssfotgxx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2opvikmrr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjcvqtd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nurnqdun.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ortzaseg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbivpvjt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vagufxsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2iggtspbl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjhuxshk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jkwzxred.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ttdzetmq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pleegjan.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cqinzisz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2sfccypwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2anlabffa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2luznnswo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oppnvppv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kswnunnu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oxixotfo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2obpdmhsb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tkbypzjq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2evuafaso.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxuouttc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yliaaacn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nkafbpta.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2alebaxxz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cyzhgheo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nqjyuywt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjpcqus.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gipzerpf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cjjycyjw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xzwnrwhy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mswcokiq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qrlkmfiu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rdorztvt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hksiujmk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xsjsiumm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jtdhkhgk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bvrmnmxy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oqfrmyvb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jyycdmks.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nppjoaqm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ecdiispr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eizjlemv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gwrkqefx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ejjoortc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2stkoyaxn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fngqmuya.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dglxqfdp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yrzdvonw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vperdsga.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufbmatwz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2iztmkwec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gasvdktg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2leftatqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtqmwpgl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2chrubrfu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2azszttjs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ssshyvow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzlqxlnv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltqasnge.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qannksku.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ilbtglan.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qwofeoax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ufryvmpt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bgeiksvp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ffmwfhbt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zuiefkrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zxdefvzi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsujlht.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ntrtjfne.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2owbywocv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wskrwoaq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjtlddk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2deaelhpe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2txlkhmbq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bbupjchk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ftfrnpbg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bkjzmvur.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bvslvhzk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iudrmpff.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kewvupad.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2riiycjpm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llufkuup.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbikkp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dviodzxw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ynppmarn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tktkiyrm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixaobtjl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgjbolc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpckeuxk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2clhrrzwp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdydbjau.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ungbbbqx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mmprzahr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ggzqghen.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2djsjnncl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okobnaqc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjrwxwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdokqqvv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kinwamqe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2liepwlnp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jcwwfesu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pjmzaktn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvkjqdjd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gctqhsbn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2spolkdyv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vbavjqxe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gmztiowt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxutac.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rdmrbaff.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksxwwlsv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wudhpddu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lufnxcla.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jrmnbwlo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfssqjo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gqckqltm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yrwosxhg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gdrmeebf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2abfpiguh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vzcczthv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nhsrcfra.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwryfyym.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ufzyizzs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2utvmkrqm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydavudhu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bplfdbdv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfpfkvaz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wlxhztog.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2prdprmmm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2aynqabaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ilfnydqi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fmowlwoc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2aehzhpwc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pjhiqjwp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2idvtkwpu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmrikplu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mgkxybie.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2otrxirrv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hllevcqa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2azmnpmuv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qtpjcbvb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hargxamu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nuseirqs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xensitlo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2alqvpjup.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2oupsypph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ptpchbdd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gkdsohqv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2naotptcx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqspigfe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hagggjop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2okgktttx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2noanlxwj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2trfhjlhz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2liciolad.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ujnvpihy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2awcalapa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dwyvambs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2oiavladm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qkbbkagb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2upnwnoxz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hwncngcm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fstaupzz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uisostyy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqfslmja.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nxtqrcgb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdttoet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vbtpztbg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyeblwae.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ymnuvjxl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2osxftjwt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tlwisips.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hmjbqhma.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zlmeiiip.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2giymgeqx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jorrrzut.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xowcuqte.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnlfpdd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqjxyvhu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oyeqnbax.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2krafggwh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2iblnuvhx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fxmhudov.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2elynstou.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fgkxrnrr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rllaitgn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dzpzarkm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zevneifl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dagqoswl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gzswabvt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tgfysbec.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kgptdvge.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vajtqzrz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jznupwte.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qxhuljvm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2emgzgymx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2putpkocl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2favfmedr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pygnvbsp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vktnvxgk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwottjf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dzawcsbf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fincxotx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhsbkqin.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xcoagitf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fzwhvmkk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwpnjgz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xjgvcnwz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2usejrova.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dxksoied.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsnasxjg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qbqyeuxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqhjkwba.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqodewlw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvoteo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gkkepefu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ufymttlb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jeihvach.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2twywzhbk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nrxwszyt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ujbyeepw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2azwpfkjq.html


<!-- 参考信息 -->