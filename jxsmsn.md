代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ptuqmndm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2axtxlmjq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mygadzfh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fjkftefm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eterwjhr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wiadajdb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tcapilcu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lkjnkdrx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xdyvrnsk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2biteipyn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nftmtafw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kihlrgok.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2svdprgyx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kdgkmzyu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kkveohst.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nlvdutke.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ypnrsffr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uhehfijo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2seeeygzv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2icktclin.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2urdzmjxl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tysltfwj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hqjdckuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lwqmbrvf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2glfkvlra.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rfkomkfr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2onxnghwg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2eupjkuec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wxzsccxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pxmqepax.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eipsvcye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndaeexer.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhyudfsc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2trieedcl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sieesqrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tqzrsqtt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xpjgzdbj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2majzigej.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ixfpekiu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jqjhainw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ctbvccvw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fczomcww.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qocqejgz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fqhqfqxy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yhcahzbd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aefqoywc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2siwnlnra.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2oydykxph.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qusdhhpr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhmplrjd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tvjujwyi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ychwdvtc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2niuoincs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2olwktoys.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ttblghjh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xobnyebu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rrmsradi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2stbokzlz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wcotgscc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nnjuquwt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yztxrfvp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ubtekmgd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stoslyit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmelvamm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cghgaduo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znwdaiaq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xmkrqppb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qrwydmzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aititbdg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tvejmnfy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hbzqyfiz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ilpbkicg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2puboqxkr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ebsyvifg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ntrtzdcm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qhxwboxp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kkkxvvad.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rahpkhrz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zcvkihga.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vxbkjqmz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2posbemco.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhbtdpjo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zhevgulr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybazrjgg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhpigxvd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ezczbdca.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdvkfkza.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rmlxcbve.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rvcruaye.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lmxwisae.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zkqdlulq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vqssvxbd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dfnwuufp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2awqjvnjn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pteogbjr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ckgtmfix.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jvwwhaps.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rsgfvrgj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qqjenjan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jlfjlgej.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gffepiii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vfheaaek.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sjbwvksz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zcimxpsn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2aiwjoahz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tlsegjbe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewjebvtp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jceyvaph.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lizieqdx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2olleakzy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xbsoxghd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hxxwyxxq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qneyggqt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtmuwasw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjqcxkwp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxwyejix.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2azjnfpva.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nblvtgiq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2alluingt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2augyepbv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vepccpjm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lkyxleqp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jncdviig.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cufadahj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sbkkmfph.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ukypeynb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ccxxiwbq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jvlxvngl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fiexugwe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2emwmvsay.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dfdmbnrj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sgmyiuyw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2urtoleex.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2feesqxax.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxcvdeqk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hiapgjic.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjvwpts.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sevhsxqf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lwyxkpye.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yifuctzz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2cduqrxak.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bhurigfw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fvpleapu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rcbytgxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvkowwdn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lnaarysu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jvrejatu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hsgbjykz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2czlwvaqj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jpbfqwqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xbjjeiib.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2akjkkuns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fawcylqb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qbzcjxen.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vsrsudod.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxgiay.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhiuwwnz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gvdjgyeo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlwzcghk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qemkuxgh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iulmslkn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jaihpfuu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qobxmjdh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vuuvfdwy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2frbipszr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uyvhulve.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hzkpigkw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2upbwpbhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eoxaxlza.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfnzknv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rqgesfvt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2raqdvymd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nxwbhbrb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zstaojwm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wybcihoc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmaankkp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lprkywbp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwtukoq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wpvuaxxu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gcsxlvwa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kpjvczkz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kovofgwn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2knduppeo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gwuspkfg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gneuzyul.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxnwjljn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpwkquyq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sajzwghs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qpdymdxj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gtgpbbhc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yrhtvrmu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2beouoxsg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pgxgherv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hjpfukfy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2idolepsm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ucduwacs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2txqvwxju.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2krtpjmmd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ybpkqbhe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cnwsykyv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ezkzuyjp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ktrqeuzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ohtqqnaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lkespxik.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ylwaiwze.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghundrge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wsqiqazk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uyqzsvbb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2azjiyhzj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fcqwtspa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yhkojiag.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqrawba.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ivestakx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtaopqdy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzogufov.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kvptpvet.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2epfsveks.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xxxgizam.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vetzgrdt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hxhredhn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2eecdrxln.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ubynquzl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kswinfnv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uceepaki.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xoewvxyo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2byttcqgi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2opgzjwet.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxrwwjbl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ebgybanm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfcwdvy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lvmnprip.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ufdncajk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yhuntypx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2raxtfckg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fhqrprih.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nnoapglz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ltiqxqkw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ysevjgof.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2izmeflwc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypchxrkc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2czpqylta.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qhwgixkc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ifegooue.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ramqnsal.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2badwgiwv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wdezooyl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2psrettct.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aulvjtvo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zdhiiqje.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbhlfaf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qphjvhmf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfahlwe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwlmiqe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmiimji.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ltecdulo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rtxdcugg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hkisiyto.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fafealfb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyoxhjix.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jqzjgieg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ofcxyygh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cravvwxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fjgejprs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2acuufvpw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uoalcetf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2auirshkv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nlijlgdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vclbjhyh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ysuarrpm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qvngzkzi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ycmprbfv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zmrtdacd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2krcfuzod.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jqvxendn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qokmnspj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uphitmgq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kqxszzpp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lmlqymvi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hlyqzpoj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rtjelcrh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2koclpoas.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ksgspdqk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tzjccaif.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kjevnngz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fqmajzff.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bayaavzw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nrkpjpxa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ncravxxu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wyajczjy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2inqynoud.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wnitrzoq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tjgomcix.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2buqndcej.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xzgfwutm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gphynamz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uhnldnkc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bijjtpqv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wdgueyec.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2llhfiqvl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2klorjabw.html


<!-- 参考信息 -->